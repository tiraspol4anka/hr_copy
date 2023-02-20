<template>
    <section class="services">
           <div class="container">
            <b-row cols="1">
                <b-col>
                    <h2 class="text-center  my-3 title_about">Подбор персонала</h2>

                </b-col>
                <b-col>
                    <div class="separate">
                        <div class="separate_center"></div>
                    </div>
                    <p class="text-center">HR Гарант рад предложить своим клиентам услугу подбора<br>
                    линейного персонала в сжатые сроки.
                    </p>
                    <p class="text-center">Мы подбираем персонал для предприятий, находящихся в Москве,<br>
                    Московской области, а также по всей территории Российской Федерации.
                    </p>
                    <p class="text-center"><b>Сферы деятельности, в которых успешно работают подобранные специалисты</b>
                    </p>
                </b-col>
            </b-row>
            <b-card-group deck>
                <b-card class="card_first  services " v-for="item in items" :key="item.id" :img-src="item.images">
                    <b-card-text class="text-center ">
                        {{ item.content }}
                    </b-card-text>
                </b-card>

            </b-card-group>
            <p class="text-center">Стоимость услуги по комплектации штата предприятия определяется <br>количеством и сложностью вакансий и обсуждается индивидуально с Заказчиком
            </p>




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
                        content: "HoReCa",
                        images: require('~/assets/images/horeca.png'),
                    },
                    {
                        id: 2,
                        content: "Производственные предприятия",
                        images: require('~/assets/images/factorys.png'),
                    },
                    {
                        id: 3,
                        content: "Строительные площадки",
                        images: require('~/assets/images/tr.png'),
                    },
                    {
                        id: 4,
                        content: "Складские комплексы",
                        images: require('~/assets/images/gr.png'),
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

    .card {

        border: 0px solid rgba(0, 0, 0, 0.125);


    }

    .card-img {
        width: 65px;
        display: block;
        margin-left: auto;
        margin-right: auto;


    }
</style>