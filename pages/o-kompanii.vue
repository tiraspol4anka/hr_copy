<template>
    <section class="about_sevice">
        <div class="container">
            <b-row cols="1">
                <b-col>
                    <h2 class="text-center  my-3 title_about">О компании</h2>
                </b-col>
                <b-col>
                    <div class="separate">
                        <div class="separate_center"></div>
                    </div>

                </b-col>
                <b-col class="text-justify">Московский кадровый центр «HR Гарант» был создан в августе 2004 года. С
                    самого основания в нашей компании трудятся
                    ответственные, высокопрофессиональные, постоянно повышающие свою квалификацию сотрудники. В
                    настоящий момент Московский
                    кадровый центр «HR Гарант» предоставляет полный спектр услуг по управлению кадровыми активами для
                    предприятий и частных
                    лиц, направленных на повышение качества работы и жизни клиентов, развития бизнеса и
                    самосовершенствования.<br><br>

                    Гарантия качества предоставляемых услуг – это наша философия.<br><br>

                    Искусно подбирая инструменты решения кадровых и экономических проблем клиента, мы всегда используем
                    индивидуальный
                    подход к каждому, учитывая все пожелания и строго соблюдая конфиденциальность.<br><br>

                    Наша компания постоянно организовывает и проводит обучающие семинары по трудовому и миграционному
                    законодательству,
                    выступает экспертом в СМИ, участвует в международных выставках.<br><br>

                    Строго следуя букве закона, безукоризненно выполняя взятые обязательства, мы стараемся поддерживать
                    и развивать деловое
                    партнерство с заказчиками, выстраивая долгосрочные и взаимовыгодные отношения.<br><br>

                    Молодой, дружный, креативный коллектив Московского кадрового центра «HR Гарант» работает для ВАС
                    честно и с
                    удовольствием!</b-col>

            </b-row>

        </div>
        <b-container class="banner" fluid>
            <div class="container">

                <b-row class="justify-content-md-center">
                    <b-col cols="12" md="6">
                        <b-img class="cert_item" src="~/assets/images/cert.png" fluid alt="" />
                        </b-img>
                    </b-col>
                    <b-col cols="10" md="4">
                        <h2 class="font-weight-normal text-white certificate">Свидетельство</h2>
                        <div class="separate-l">
                            <div class="separate-center-l"></div>
                        </div>
                        <p class="text-white">Свидетельство о том, что Гарант является членом
                            территориального объединения работодателей
                            «Организация Московской Конференции
                            промышленников и предпринимателей Западного
                            административного округа города Москвы»</p>



                    </b-col>

                </b-row>

            </div>

        </b-container>
        <h6 class="text-center mcc">Наша компания оказывает следующие услуги:</h6>
        <Service />
    </section>
</template>

<style>
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

    .banner {
        background-image: url(~/assets/images/slide-img-blur.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
        width: 100%;
        bottom: 0;
        z-index: 1;
    }

    .separate-l {
        width: 20%;
        height: 1px;
        background: #808080;
        margin-left: inherit;
        margin-right: auto;
        margin-top: 20px;
        margin-bottom: 30px;
    }

    .separate-center-l {
        width: 6%;
        height: 3px;
        background: red;
        position: absolute;
        left: 7%;
        margin-top: -1px;
    }

    .cert_item {
        padding-top: 20px;
        padding-bottom: 20px;
    }

    .certificate {
        padding-top: 60px;
    }
     .mcc {
    font-weight: 400;
    font-size: 1.2em;
    padding-top: 100px;
    padding-bottom: 80px;
    font-family: 'Segoe UI', Arial, sans-serif;
  }
</style>