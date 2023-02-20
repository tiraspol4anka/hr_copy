<template>
    <section class="banner">
        <div class="container">
            <b-container fluid>
                <b-row>
                    <b-col class="banner_img">
                        <b-container>
                            <b-row>
                                <b-col>
                                    <b-container>
                                        <b-row class="text-center items_number">
                                            <b-col><span class="number">15</span><br>
                                                <span class="number_info">лет успешной работы</span>

                                            </b-col>

                                            <b-col><span class="number">100 </span><br>
                                                <span class="number_info">легализованных работников</span>
                                            </b-col>
                                            <b-col><span class="number">650</span><br>
                                                <span class="number_info"> довольных клиентов</span>
                                            </b-col>
                                        </b-row>
                                    </b-container>
                                </b-col>

                            </b-row>
                        </b-container>
                    </b-col>

                </b-row>
            </b-container>
        </div>
    </section>
</template>

<style scoped>
    .banner {
        background-image: url(~/assets/images/slide-img-blur.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
        width: 100%;
        bottom: 0;
        z-index: 1;
    }

    .banner_img {
        background-image: url(~/assets/images/bg-calc.png);
        background-repeat: no-repeat;
        height: 241px;
        width: 100%;
        margin: 2% 0px;
        background-size: contain;
        background-position: center;
        position: relative;
    }

    .number {
        font-size: 100px;
        color: rgba(255, 255, 255, 0.8);

    }

    .number_info {
        font-size: 16px;
        color: rgba(255, 255, 255, 0.8);

    }

    @media screen and (max-width: 768px) {
        .number {
            font-size: 22px;

        }

        .number_info {
            font-size: 11px;
            display: block;
            margin-top: -11px;
        }

        .items_number {
            margin-top: 90px;
            margin-left: -39px;
            margin-right: -39px;

        }
    }
</style>