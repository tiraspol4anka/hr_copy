<template>

    <article>
        <b-container fluid style="background-color: white;">
            <b-row>
                <b-col md="2"></b-col>
                <b-col md="8">
                    <nuxt-content :document="article" />
                    <nuxt-link to="/news/"><button class="about backnews">Назад к новостям</button></nuxt-link>
                </b-col>
                <b-col md="2"></b-col>
            </b-row>
        </b-container>
    </article>
</template>




<script>
    export default {
        async asyncData({ $content, params }) {
            const article = await $content('news', params.slug).fetch()

            return { article }
        }

    }
</script>

<style>
    .date-news {
        color: darkgrey;
        font-size: 14px;
    }

    .backnews {
        margin-bottom: 20px;
        margin-left: -13px;
    }

    .about {
        float: left;
        border: 0px;
        background: rgba(0, 0, 0, 0.45);
        padding: 5px 20px 5px 20px;
        color: white;
        border-bottom: 1px solid rgba(0, 0, 0, 0);
        cursor: pointer;
    }

    .backnews:hover {
        background-color: #a3100b;
        color: white;
    }

    div.news-detail img.detail_picture {
        float: left;
        margin: 0 8px 6px 1px;
    }

    .detail_picture {
        width: 50%;
        height: auto;
    }
</style>