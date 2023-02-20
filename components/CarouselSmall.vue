<template>
    <section class="small_carousel">
        <div class="container-fluide banner">
            <b-container class="bv-example-row">
                <h2 class="our_clients">Наши клиенты</h2>
                <div class="banner__line">
                    <div class="banner__line-middle"></div>
                </div>
                <b-row>
                    <b-col class="items_clients">
                        <div class="carousel-wrapper">
                            <client-only>
                                <slick :options="slickOptions">
                                    <div v-for="i in 22" :key="i" class="img-wrapper">
                                        <img :src="`./images/${i}.png`" />
                                    </div>
                                </slick>
                            </client-only>
                        </div>
                    </b-col>
                </b-row>
            </b-container>
        </div>
    </section>
</template>

<script>

    export default {
        data() {
            return {
                slickOptions: {

                    slidesToShow: 5,
                    autoplay: true,
                    autoplaySpeed: 1000,
                    arrows: false,
                    responsive: [
                        {
                            breakpoint: 1024,
                            settings: {
                                slidesToShow: 3,
                                slidesToScroll: 3,
                                infinite: true,
                                
                            }
                        },
                        {
                            breakpoint: 600,
                            settings: {
                                slidesToShow: 2,
                                slidesToScroll: 2
                            }
                        },
                        {
                            breakpoint: 480,
                            settings: {
                                slidesToShow: 2,
                                slidesToScroll: 1
                            }
                        }
                    ]
                }
                
            }
        }
    }
</script>

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

    .our_clients {
        font-size: 32px;
        color: white;
        text-align: center;
        font-weight: 400;
        padding-top: 80px;
        
    }

    

    .banner__line-middle {
        width: 3%;
        left: 49%;
       
    }

    .carousel-wrapper {
        padding: 10px;

    }

    .img-wrapper img {
        margin: auto;
        width: 150px;
        height: 100px;
        filter: grayscale(100%);

    }

    .img-wrapper img:hover {
        
        filter: grayscale(0);
        cursor: pointer;

    }
    
    .items_clients{
        padding-top: 60px;
        padding-bottom: 60px;
    }
</style>