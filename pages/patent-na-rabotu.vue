<template>
    <section class="patent">
      
   
<div class="container">
    <b-row cols="1">
        <b-col>
            <h2 class="text-center  my-3 title_about">Патент на работу для иностранных граждан⁠</h2>

        </b-col>
        <b-col>
            <div class="separate">
                <div class="separate_center"></div>
            </div>
            <p class="text-center">Московский кадровый центр «HR Гарант» оказывает содействие в оформлении полного пакета<br> документов для получения патентов
            включая:
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
<p class="text-center">После получения пакета документов, на нашем фирменном автобусе мы отвезем иностранных граждан в ММЦ Сахарово, где они
без очереди подадут документы на получение патента и комфортно пройдут процедуру дактилоскопии в присутствии нашего
специалиста.
</p>




</div>
<Docs />

</section>

</template>

<script>
    export default {
        data() {
            return {
                items: [
                    {
                        id: 1,
                        content: "Нотариальный перевод паспорта",
                        images: require('~/assets/images/oformlenie_patenta_img1.png'),
                    },
                    {
                        id: 2,
                        content: "Полис Добровольного Медицинского Страхования (ДМС)",
                        images: require('~/assets/images/oformlenie_patenta_img2.png'),
                    },
                    {
                        id: 3,
                        content: "Медицинские справки",
                        images: require('~/assets/images/oformlenie_patenta_img3.png'),
                    },
                    {
                        id: 4,
                        content: "Сертификат о знании Русского языка",
                        images: require('~/assets/images/oformlenie_patenta_img3.png'),
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
    width: 120px;
    display: block;
    margin-left: auto;
    margin-right: auto;


  }
</style>

