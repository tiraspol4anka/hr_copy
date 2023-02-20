<template>
  <div>
    <CarouselBig />
    <h2 class="text-center mcc">Московский кадровый центр «HR Гарант» предоставляет<br> следующие услуги для крупных
      компаний<br> и малых предприятий:</h2>
    <Service />
    <BannerNumbers />
    <ServiceUseful />
    <CarouselSmall />
    
    <HrGarant />
  </div>
</template>

<script>
  export default {}
</script>

<style>
  body {
    font-family: "Segoe UI", Arial, sans-serif;
  }

  .title {
    font-family:
      'Segoe UI',
      Roboto,
      'Helvetica Neue',
      Arial,
      sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
    background-image: url(~/assets/images/bg-paper.png);
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    padding-top: 15px;
  }

  .mcc {
    font-weight: 400;
    font-size: 1.2em;
    padding-top: 100px;
    padding-bottom: 80px;
    font-family: 'Segoe UI', Arial, sans-serif;
  }
</style>