<template>
    <section class="services">
        <div class="container">
        <b-row cols="1">
            <b-col>
                <h2 class="text-center  my-3 title_about">Услуги</h2>
            </b-col>
            <b-col>
                <div class="separate">
                    <div class="separate_center"></div>
                </div>
            </b-col>
        </b-row>
        </div>
        <Service />
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
    .services {
        background-image: url(~/assets/images/bg-paper.png);
    }
      

    .title_about {
        font-weight: 400;
    }

    .separate {
        width: 20%;
        height: 1px;
        background: #808080;
        margin-left: auto;
        margin-right: auto;
        margin-top: 20px;
        margin-bottom: 30px;
    }

    .separate_center {
        width: 6%;
        height: 3px;
        background: red;
        position: absolute;
        left: 47%;
        margin-top: -1px;
    }


    .center {
        width: 65px;

    }

    .mcc {
        font-weight: 400;
        padding-top: 100px;
        padding-bottom: 80px;
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