<template>
    <section class="items__carousel" style="max-width:100vw;">

        <b-carousel id="carousel-fade" v-model="slide" :interval="0" fade controls indicators
            @sliding-start="onSlideStart" @sliding-end="onSlideEnd">
            <b-carousel-slide style="height:620px" class="slider_one">
                <b-container>
                    <b-row>
                        <b-col>
                            <h1 class="banner_title">Аутстаффинг персонала</h1>
                        </b-col>
                    </b-row>
                    <div class="banner__line">
                        <div class="banner__line-middle"></div>
                    </div>
                    <b-row>
                        <b-col>
                            <p>Вывод сотрудников за штат - идеальное решение для найма трудовых мигрантов</p>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col class="items__banner">
                            <b-row>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon1.png" />
                                    </b-img>
                                </b-col>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon2.png" />
                                    </b-img>
                                </b-col>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon3.png" />
                                    </b-img>
                                </b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col class="items__banner">
                            <b-row>
                                <b-col>Сокращение издержек</b-col>
                                <b-col>Отсутствие трудовых споров</b-col>
                                <b-col>Оптимизация налогообложения</b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col>
                            <p style="padding-top: 40px;">Полный комплекс услуг для работодателя, использующего<br>
                                российскую и иностранную рабочую силу</p>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col>
                            <div>
                                <span><button class="zak callme">Заказать</button></span>
                                <span>
                                    <nuxt-link to="/autstaffing"><button class="about_button">Подробнее</button>
                                    </nuxt-link>
                                </span>
                            </div>
                        </b-col>
                    </b-row>
                </b-container>
            </b-carousel-slide>
            <b-carousel-slide style="height:620px" class="slider_second">
                <b-container>
                    <b-row>
                        <b-col>
                            <h1 class="banner_title">Миграционный аудит</h1>
                        </b-col>
                    </b-row>
                    <div class="banner__line">
                        <div class="banner__line-middle"></div>
                    </div>
                    <b-row>
                        <b-col>
                            <p>Проверка соблюдения миграционного законодательства и оформления иностранных работников
                            </p>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col class="items__banner">
                            <b-row>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon21.png" />
                                    </b-img>
                                </b-col>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon22.png" />
                                    </b-img>
                                </b-col>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon23.png" />
                                    </b-img>
                                </b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col class="items__banner">
                            <b-row>
                                <b-col>Первичная консультация</b-col>
                                <b-col>Проверка кадровой документации</b-col>
                                <b-col>Проверка подлинности документов</b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col>
                            <p style="padding-top: 30px;">Полный комплекс услуг для работодателя, использующего<br>
                                российскую и иностранную рабочую силу</p>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col>
                            <div>
                                <span><button class="zak callme">Заказать</button></span>
                                <span>
                                    <nuxt-link to="/migratsionnyy-audit"><button class="about_button">Подробнее</button>
                                    </nuxt-link>
                                </span>
                            </div>
                        </b-col>
                    </b-row>
                </b-container>
            </b-carousel-slide>
            <b-carousel-slide style="height:620px" class="slider_third">
                <b-container>
                    <b-row>
                        <b-col>
                            <h1 class="banner_title">Патент на работу</h1>
                        </b-col>
                    </b-row>
                    <div class="banner__line">
                        <div class="banner__line-middle"></div>
                    </div>
                    <b-row>
                        <b-col>
                            <p>Оформлении полного пакета документов для получения патентов на работу</p>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col class="items__banner">
                            <b-row>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon31.png" />
                                    </b-img>
                                </b-col>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon32.png" />
                                    </b-img>
                                </b-col>
                                <b-col>
                                    <b-img v-bind="mainProps" class="banner__img" src="~/assets/images/icon33.png" />
                                    </b-img>
                                </b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col class="items__banner">
                            <b-row>
                                <b-col>Нотариальный перевод паспорта</b-col>
                                <b-col>Полис ДМС и медицинские справки</b-col>
                                <b-col>Сертификат о знании Русского языка</b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col>
                            <p style="padding-top: 40px;">Полный комплекс услуг для работодателя, использующего <br>
                                российскую и иностранную рабочую силу</p>
                        </b-col>
                    </b-row>
                    <b-row>
                        <b-col>
                            <div>
                                <span><button class="zak callme">Заказать</button></span>
                                <span>
                                    <nuxt-link to="/patent-na-rabotu"><button class="about_button">Подробнее</button>
                                    </nuxt-link>
                                </span>
                            </div>
                        </b-col>
                    </b-row>
                </b-container>
            </b-carousel-slide>
        </b-carousel>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                slide: 0,
                sliding: null,

                mainProps: { width: 100, height: 100, class: 'm1' }
            }
        },
        methods: {
            onSlideStart(slide) {
                this.sliding = false
            },
            onSlideEnd(slide) {
                this.sliding = false
            }


        }
    }
</script>
<style>
    .slider_one {
        background: url("~/assets/images/slide-2-img.jpg");
        height: 620px;
        background-size: cover;
    }

    .slider_second {
        background: url("~/assets/images/slide-2.png");
        height: 620px;
        background-size: cover;

    }

    .slider_third {
        background: url("~/assets/images/slide-3.png");
        height: 620px;
        background-size: cover;
    }

    .carousel-caption {
        bottom: 94px;
       right: 10%;
       left: 10%;
    }

    .banner_title {
        text-align: center;
        color: white;
        padding-top: 60px;
        font-size: 2.5rem;
        font-weight: 100;


    }

    .banner__line {
        width: 20%;
        height: 1px;
        background: #808080;
        margin-left: auto;
        margin-right: auto;
        margin-top: 20px;
        margin-bottom: 30px;
    }

    .banner__line-middle {
        width: 6%;
        height: 3px;
        background: red;
        margin-top: -1px;
        left: 47%;
        position: absolute;
    }

    .zak {

        border: 0px;
        background: #ee2738;
        color: white;
        border-bottom: 1px solid #b11f29;
        cursor: pointer;
    }

    .zak:hover {
        background-color: #a3100b;
    }

    .about_button {

        border: 0px;
        background: rgba(0, 0, 0, 0.45);

        color: white;
        border-bottom: 1px solid rgba(0, 0, 0, 0);
        cursor: pointer;
    }

    .about_button:hover {
        background-color: #a3100b;

    }

    @media screen and (max-width: 768px) {
        .items__banner {
            display: none;
        }

        .items__carousel {
            margin: 0px !important;
            padding: 0px !important;
            width: 100% !important;
        }
    }
</style>