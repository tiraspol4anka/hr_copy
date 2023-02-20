<template>
    <section class="services">
        <div class="container">
            <b-card-group deck>
                <b-card class="services" v-for="item in items" :key="item.id" :img-src="item.images">
                    <b-card-text class="text-center "><b class="title_service">{{ item.name }}</b>
                    </b-card-text>
                    <b-card-text class="text-center">
                        {{ item.description }}
                    </b-card-text>

                    <b-card-text class="text-center">
                        <nuxt-link :to="`/${item.link}`"> <button class="zak">{{item.button}}</button></nuxt-link>
                    </b-card-text>
                </b-card>
            </b-card-group>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                items: [
                    {
                        id: 1,
                        name: "АУТСТАФФИНГ",
                        description: "вывод персонала за штат с целью оптимизации расходов",
                        link: 'autstaffing',
                        images: require('~/assets/images/main-1.svg'),
                        button: 'Подробнее'
                    },
                    {
                        id: 2,
                        name: "МИГРАЦИОННЫЙ АУДИТ",
                        description: "это анализ предприятий, направленный на проверку соблюдения миграционного законодательства",
                        link: "migratsionnyy-audit",
                        images: require('~/assets/images/main-2.svg'),
                        button: 'Подробнее'
                    },
                    {
                        id: 3,
                        name: "КОНСАЛТИНГ",
                        description: "Экономический расчёт и финансовое моделирование первичны при создании бизнеса и управлении им.",
                        link: "konsalting",
                        images: require('~/assets/images/icon4.png'),
                        button: 'Подробнее'
                    },
                    {
                        id: 4,
                        name: "ПОДБОР ПЕРСОНАЛА",
                        description: "подбор работников для реализации любых задач",
                        link: "podbor-personala",
                        images: require('~/assets/images/icon5.png'),
                        button: 'Подробнее'
                    },
                ],
            };
        },
    }
</script>

<style scoped>
    .services {
        background-image: url(~/assets/images/bg-paper.png);
    }

    .title_service {
        font-weight: 500;
    }

    .center {
        width: 65px;

    }

    .mcc {
        font-weight: 400;
        font-size: 1.2em;
        padding-top: 100px;
        padding-bottom: 80px;
        font-family: 'Segoe UI', Arial, sans-serif;
    }

    .card-img {
        width: 65px;
        display: block;
        margin-left: auto;
        margin-right: auto;


    }

    .card {

        border: 0px solid rgba(0, 0, 0, 0.125);

    }

    .service__link {

        border: 0px;
        background: #ee2738;
        padding: 5px 20px 5px 20px;
        color: white;
        border-bottom: 1px solid #b11f29;
        cursor: pointer;
        margin-left: auto;
        margin-right: auto;
        margin-top: 25px;


    }
</style>