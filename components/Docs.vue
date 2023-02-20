<template>

    <b-container fluid style="background-color: white;">
        <div class="container">
            <b-row cols="1">
                <b-col>
                    <h2 class="text-center  my-3 title_about">Документы необходимые для оформления патента на работу⁠
                    </h2>
                </b-col>
                <b-col>
                    <div class="separate">
                        <div class="separate_center"></div>
                    </div>
                    <p class="text-center">подаются в органы УФМС в течение 30 календарных дней со дня въезда на
                        территорию РФ
                    </p>
                </b-col>
            </b-row>
            <b-card-group deck>
                <b-card class="services mt-3" v-for="item in items" :key="item.id" :img-src="item.images">
                    <b-card-text class="text-center">
                        {{ item.content }}
                    </b-card-text>
                </b-card>
            </b-card-group>
        </div>
    </b-container>
</template>

<script>
    export default {
        data() {
            return {
                items: [
                    {
                        id: 1,
                        content: "Загранпаспорт иностранного гражданина",
                        images: require('~/assets/images/translation-passport-ico.jpg'),
                    },
                    {
                        id: 2,
                        content: "Миграционная карта",
                        images: require('~/assets/images/migration-card-ico.jpg'),
                    },
                    {
                        id: 3,
                        content: "Нотариальный перевод паспорта",
                        images: require('~/assets/images/cert-translate-pass-ico.jpg'),
                    },
                    {
                        id: 4,
                        content: "Регистрация",
                        images: require('~/assets/images/register-ico.jpg'),
                    },
                    {
                        id: 5,
                        content: "Фото 3*4 цветные матовые на белом фоне, 2 шт.",
                        images: require('~/assets/images/doc-photo-ico.jpg'),
                    },
                    {
                        id: 6,
                        content: "Полис Добровольного Медицинского Страхования",
                        images: require('~/assets/images/oformlenie_patenta_img2.png'),
                    },
                    {
                        id: 7,
                        content: " Сертификат о знании Русского языка",
                        images: require('~/assets/images/rus-lang-cert-ico.jpg'),
                    },
                    {
                        id: 8,
                        content: "Мед комиссия",
                        images: require('~/assets/images/med-board-ico.jpg'),
                    },
                    {
                        id: 9,
                        content: "Квитанция об уплате гос пошлины (по г. Москве 4 500 руб.)",
                        images: require('~/assets/images/receipt-ico.jpg'),
                    },

                ],
            };
        },
    }
</script>

<style scoped>
    .card {

        border: 0px solid rgba(0, 0, 0, 0.125);
        flex: 1 0 23%;

    }

    .card-img {
        width: 120px;
        display: block;
        margin-left: auto;
        margin-right: auto;


    }
</style>