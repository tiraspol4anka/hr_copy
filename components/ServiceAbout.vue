<template>
    <section class="services">
        <div class="container">
            <b-card-group deck>
                <b-card class="services" v-for="item in items" :key="item.id" :img-src="item.images">
                    <b-card-text class="text-center">
                        {{ item.name }}
                    </b-card-text>
                    <b-card-text class="text-center">
                        {{ item.description }}
                    </b-card-text>
                    <a>
                        <b-card-text class="service__link text-center">
                            {{ item.button }}
                        </b-card-text>
                    </a>
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
                        button: "ПОДРОБНЕЕ",
                        images: require('~/assets/images/main-1.svg'),
                    },
                    {
                        id: 2,
                        name: "МИГРАЦИОННЫЙ АУДИТ",
                        description:
                            "это анализ предприятий, направленный на проверку соблюдения миграционного законодательства",
                        button: "ПОДРОБНЕЕ",
                        images: require('~/assets/images/main-2.svg'),
                    },
                    {
                        id: 3,
                        name: "КОНСАЛТИНГ",
                        description:
                            "Экономический расчёт и финансовое моделирование первичны при создании бизнеса и управлении им.",
                        button: "ПОДРОБНЕЕ",
                        images: require('~/assets/images/icon4.png'),
                    },
                    {
                        id: 4,
                        name: "ПОДБОР ПЕРСОНАЛА",
                        description: "подбор работников для реализации любых задач",
                        button: "ПОДРОБНЕЕ",
                        images: require('~/assets/images/icon5.png'),
                    },
                ],
            };
        },
    }
</script>

<style scoped>
    .center {
        width: 65px;


    }

    .card-img {
        width: 65px;
        display: block;
        margin-left: auto;
        margin-right: auto;


    }

    .card {

        border: 0px solid rgba(0, 0, 0, 0.125);
        background-color: transparent;

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

    .our_company_title {
        padding-top: 80px;
        padding-bottom: 40px;
    }

    .text-center {
        font-weight: 500;
    }
</style>