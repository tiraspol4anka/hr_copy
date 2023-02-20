<template>
    <div class="container">
        <b-row cols="1">
            <b-col>
                <h2 class="text-center  my-3 title_about">Новости</h2>
            </b-col>
            <b-col>
                <div class="separate">
                    <div class="separate_center"></div>
                </div>

            </b-col>
        </b-row>
        <b-row class="justify-content-md-center news-item"
            v-for="article in articles.slice((currentPage-1)*perPage,(currentPage-1)*perPage+perPage)" :key="article.id"
            :per-page="perPage" :current-page="currentPage">
            <b-col cols="12" md="4">
            <nuxt-link :to="`/news/${article.slug}/`"> <b-img :src="require(`~/assets/images/news/${article.img}`)"  fluid style="height: 165px; width: 280px;">
                </b-img></nuxt-link>
            </b-col>
            <b-col cols="10" md="6" class="news_description">
                <h6 class="title_information">{{ article.title }}</h6>
                <p class="text-black-50">{{ article.date }}</p>

                <p>{{ article.description }}</p>
                <nuxt-link :to="`/news/${article.slug}/`"><span><button class="zak callme">Прочитать</button></span></nuxt-link>

            </b-col>
        </b-row>
        <b-pagination align="center" v-model="currentPage" :total-rows="rows" :per-page="perPage">
        </b-pagination>
    </div>
</template>

<script>
    export default {
        async asyncData({ $content, params }) {

            const articles = await $content('news', params.slug)
                .sortBy("data")

                .fetch();



            return {
                perPage: 20,
                currentPage: 1,

                articles
            }
        },
        computed: {
            rows() {
                return this.articles.length
            }
        }

    }
</script>
<style scoped>
    .title_information {
        margin-top: 20px;
    }

    .news-item {

        border-bottom: 1px solid #d6d6d6;
        padding-top: 35px;
        padding-bottom: 35px;
    }
    .news_description{
        margin-top: -22px;
    }
</style>