<template>
    <section class="services">
        <div class="container">
            <b-row cols="1">
                <b-col>
                    <h2 class="text-center  my-3 title_about">Цены</h2>
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
                        <th scope="row">Aутстаффинг</th>
                        <td></td>
                        <td>от 800 рублей</td>
                    </tr>
                    <tr>
                        <th scope="row">Миграционный аудит</th>
                            <td>1-5 человек<br>
                                6-10 человек<br>
                                10-20 человек<br>
                                более 20 человек<br>
                            </td>
                            <td>2000 рублей<br>
                                1500 рублей<br>
                                850 рублей<br>
                                по договоренности<br>
                            </td>
                    </tr>
                    <tr>
                        <th scope="row">Подбор персонала</th>
                        <td>от 5 человек</td>
                        <td>от 2500 рублей</td>
                    </tr>
                    <tr>
                        <th scope="row">Патент на работу</th>
                        <td>патент по Москве<br>
                            патент по Московской области
                        </td>
                        <td>от 11 700 руб<br>
                            от 22 000 руб
                        </td>
                    </tr>
                    <tr>
                        <th scope="row">Cеминары</th>
                        <td>семинары-практикумы по миграционному и<br>
                            трудовому законодательству
                        </td>
                        <td>бесплатно</td>
                    </tr>
                </tbody>
            </table>

        </div>

    </section>
</template>


<script>

</script>


<style>
    @media screen and (max-width: 768px){
     .table {
        font-size: 11px;
     }
}

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
</style>