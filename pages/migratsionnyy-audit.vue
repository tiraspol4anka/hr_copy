<template>
  <section class="services">
    <div class="container">
      <b-row cols="1">
        <b-col>
          <h2 class="text-center  my-3 title_about">Миграционный аудит</h2>

        </b-col>
        <b-col>
          <div class="separate">
            <div class="separate_center"></div>
          </div>
          <p class="text-center">Миграционный аудит – это новое направление аудита предприятий всех форм собственности,
            <br>направленный на проверку соблюдения миграционного законодательства и правильности<br>кадрового
            оформления иностранных работников, прибывших на
            территорию РФ.</p>
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

    <b-container fluid class="home_three_bg">
      <div class="container">
        <b-row>
          <b-col>
            <h2 class="text-center text-white">Штрафные меры для<br> юридических лиц</h2>
          </b-col>
        </b-row>
        <b-row class="text-white">
          <b-col md="4">
            <p class="san san-line">800 000 - <br> 1 000 000 руб.</p>
            <p>За каждого мигранта</p>

          </b-col>
          <b-col md="4">
            <p class="san san-line">45 000 -<br> 50 000 руб.</p>
            <p>На руководителя компании</p>

          </b-col>
          <b-col md="4">
            <p class="san">90 суток</p>
            <p>приостановление деятельности компании</p>

          </b-col>
        </b-row>

      </div>
    </b-container>
<div class="container">
    <b-row cols="1">
      <b-col>
        <h2 class="text-center  my-3 title_about">Стоимость миграционного аудита</h2>

      </b-col>
      <b-col>
        <div class="separate">
          <div class="separate_center"></div>
        </div>

      </b-col>
    </b-row>

<table class="table">
  <tbody>
    <tr>
      <td>1</td>
      <td>миграционный аудит</td>
      <td>1-5 человек</td>
      <td>2000 рублей</td>
    </tr>
    <tr>
      <td>2</td>
      <td>миграционный аудит</td>
      <td>6-10 человек</td>
      <td>1500 рублей</td>
    </tr>
  <tr>
    <td>3</td>
    <td>миграционный аудит</td>
    <td>10-20 человек</td>
    <td>850 рублей</td>
  </tr>
  <tr>
    <td>4</td>
    <td>миграционный аудит</td>
    <td>более 20 человек</td>
    <td>по договоренности
</td>
  </tr>
  </tbody>
</table>

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
            content: "Первичная консультация по вопросам привлечения и использования иностранной рабочей силы.",
            images: require('~/assets/images/icon_c.png'),
          },
          {
            id: 2,
            content: "Проверка всей кадровой документации, необходимой для оформления на работу иностранных граждан.",
            images: require('~/assets/images/icon_d.png'),
          },
          {
            id: 3,
            content: "Заключение о выявленных нарушениях в области миграционного законодательства и рекомендации по их устранению.",
            images: require('~/assets/images/icon_de.png'),
          },
          {
            id: 4,
            content: "Выезд специалиста на Ваше предприятие. Личное общение дает преимущества в понимании ситуации",
            images: require('~/assets/images/icon_ca.png'),
          },
          {
            id: 5,
            content: "Проверка подлинности документов иностранных граждан (миграционной карты, патента и других документов)",
            images: require('~/assets/images/icon_dc.png'),
          }

        ],
      };
    },
  }
</script>


<style scoped>
  @media screen and (max-width: 768px) {
    .table {
      font-size: 11px;
    }
  }

  .home_three_bg {
    background: url(~/assets/images/slide-img-blur.jpg) center no-repeat;
    background-size: cover;
    position: relative;
    width: 100%;
    bottom: 0;
    z-index: 1;
  }


  

  .services {

    background-image: url(~/assets/images/bg-paper.png);
  }


  .center {
    width: 65px;

  }

  .mcc {
    font-weight: 1.2em;
    padding-top: 100px;
    padding-bottom: 80px;
    font-family: 'Segoe UI', Arial, sans-serif;
  }

  .card-img {
    width: 65px;
    display: block;
    margin-left: auto;
    margin-right: auto;


  }

  .card {

    border: 0px solid rgba(0, 0, 0, 0.125);
    flex: 1 0 23%;
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

  .san-line {
    border-right: 1px solid rgba(255, 255, 255, 0.6);
  }

  .san {
    color: white;
    font-size: 40px;
    line-height: 1;
    margin-bottom: 0px;
    margin-top: 20px;
  }
</style>