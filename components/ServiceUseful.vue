<template>
    <section class="services">
        <div class="container">
            <h1 class="text-center mcc">Наши услуги будут полезны</h1>
            <b-card-group deck>
                <b-card class="services" img-src="~/assets/images/icon6.png">
                    <b-card-text class="text-center">
                        <b class="title_service">Генеральному директору</b>
                    </b-card-text>
                    <b-card-text class="text-center">
                        Возможность сосредоточиться на ключевых моментах бизнеса
                    </b-card-text>
                    <b-card-text class="text-center">
                        <button v-b-modal="'1'" class="zak">Подробнее</button>
                        <b-modal id="1" size="xl" hide-footer>
                            <template>
                                <h5 class="text-center">Преимущества для генерального директора</h5>
                                <div class="separate">
                                    <div class="separate_center"></div>
                                </div>

                            </template>
                            <b-row class="text-center">
                                <b-col md="6">
                                    <img src="~/assets/images/2.svg" class="finver">
                                    <p>Снижение затрат за счет экономии на заработной плате и налогах внутренних
                                        сотрудников, рабочих местах, площадях.</p>
                                </b-col>

                                <b-col md="6"><img src="~/assets/images/3.svg" class="finver">
                                    <p>Отсутствие необходимости оборудовать места хранения трудовых книжек и иных
                                        кадровых документов</p>
                                </b-col>

                            </b-row>
                            <div class="text-center"><button class="zak">Оставить заявку</button></div>
                        </b-modal>
                    </b-card-text>

                </b-card>
                <b-card class="services" img-src="~/assets/images/icon7.png">
                    <b-card-text class="text-center">
                        <b class="title_service">Главному бухгалтеру</b>
                    </b-card-text>
                    <b-card-text class="text-center">
                        Перенос большой части затрат из статьи ‘Расхода на заработную плату’ в статью ‘Услуги’
                    </b-card-text>
                    <b-card-text class="text-center">
                        <button v-b-modal="'2'" variant="primary" class="zak">Подробнее</button>
                        <b-modal id="2" size="xl" hide-footer>
                            <template>
                                <h5 class="text-center">Преимущества для главного бухгалтера</h5>
                                <div class="separate">
                                    <div class="separate_center"></div>
                                </div>

                            </template>
                            <b-row class="text-center">
                                <b-col md="6">
                                    <img src="~/assets/images/5.svg" class="finver">
                                    <p>Снижение документооборота до одной счет-фактуры в месяц вместо расчетных
                                        ведомостей и отчетностей по з/п</p>
                                </b-col>

                                <b-col md="6"><img src="~/assets/images/6.svg" class="finver">
                                    <p>За счет фиксированной комиссии нет необходимости ограничивать рост заработной
                                        платы сотрудников, передаваемых на
                                        аутстаффинг.</p>
                                </b-col>

                            </b-row>
                            <div class="text-center"><button class="zak">Оставить заявку</button></div>
                        </b-modal>
                    </b-card-text>
                </b-card>
                <b-card class="services" img-src="~/assets/images/icon8.png">
                    <b-card-text class="text-center">
                        <b class="title_service">Руководителю кадрового подразделения</b>
                    </b-card-text>
                    <b-card-text class="text-center">
                        Снижение штатной численности сотрудников компании
                    </b-card-text>
                    <b-card-text class="text-center">
                        <button v-b-modal="'3'" variant="primary" class="zak">Подробнее</button>
                        <b-modal id="3" size="xl" hide-footer>
                            <template>
                                <h5 class="text-center">Преимущества для руководителя кадрового подразделения</h5>
                                <div class="separate">
                                    <div class="separate_center"></div>
                                </div>

                            </template>
                            <b-row class="text-center">
                                <b-col md="6">
                                    <img src="~/assets/images/7.svg" class="finver">
                                    <p>Снижение штатной численности сотрудников вашей организации
                                    </p>
                                </b-col>

                                <b-col md="6"><img src="~/assets/images/8.svg" class="finver">
                                    <p>Отсутствие риска трудовых споров, так как работодателем выступает стороннее
                                        юридическое лицо</p>
                                </b-col>

                            </b-row>
                            <div class="text-center"><button class="zak">Оставить заявку</button></div>
                        </b-modal>
                    </b-card-text>
                </b-card>
            </b-card-group>
        </div>
    </section>
</template>

<style>
    .modal-header {
        border-bottom: 0px solid #dee2e6;

    }

    .finver {
        filter: invert(0.9);
    }
</style>


<style scoped>
    .services {
        background-image: url(~/assets/images/bg-paper.png);
    }

    .center {
        width: 65px;

    }

    .mcc {
        font-weight: 400;
        padding-top: 100px;
        padding-bottom: 80px;
        font-size: 1.2em;
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

    .card-deck {
        padding-bottom: 100px;
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

    .title_service {
        font-weight: 500;
    }
</style>