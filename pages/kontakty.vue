<template>
    <section class="services">
        <div class="container">
            <b-row cols="1">
                <b-col>
                    <h2 class="text-center  my-3 title_about">Контакты</h2>
                </b-col>
                <b-col>
                    <div class="separate">
                        <div class="separate_center"></div>
                    </div>

                </b-col>
            </b-row>
        
            
            <b-row class="mb-3">
                <b-col md="6">
                    <div class="map" style="position:relative;overflow:hidden;"><a
                        href="https://yandex.ru/maps/213/moscow/?utm_medium=mapframe&utm_source=maps"
                        style="color:#eee;font-size:12px;position:absolute;top:0px;">Москва</a><a
                        href="https://yandex.ru/maps/213/moscow/?from=api-maps&ll=37.453908%2C55.710731&mode=usermaps&origin=jsapi_2_1_78&um=constructor%3A195b64111e8becab6bc2c8f6aae91e509131e9a06c3f300348284a2792a703cb&utm_medium=mapframe&utm_source=maps&z=11"
                        style="color:#eee;font-size:12px;position:absolute;top:14px;">Яндекс.Карты — транспорт,
                        навигация, поиск
                        мест</a><iframe src="https://yandex.ru/map-widget/v1/-/CCUmy4RswA" width="550px" height="650px" frameborder="0"
                        allowfullscreen="true" style="position:relative;" class="map"></iframe>
                    </div>
                </b-col>
                <b-col md="6">
                 <h6>Контактная информация</h6>
                 <div class="item_inf">
                    <p><b-icon icon="geo-alt-fill" style="color: #ee2738;"></b-icon>Адрес: 121357, Москва, улица Ватутина, 11</p>
                    <p><b-icon icon="geo-alt-fill" style="color: #ee2738;"></b-icon>Адрес: 191144, Санкт Петербург, улица Мытнинская, д. 12/44</p>
                    <p><b-icon icon="telephone-fill" style="color: #ee2738;"></b-icon>Телефон: +7 (495) 118-33-83</p>
                    <p><b-icon icon="envelope" style="color: #ee2738;"></b-icon>Email: sale@hrgarant.ru</p>
                    <p><b-icon icon="envelope" style="color: #ee2738;"></b-icon>Email: platonov@hrgarant.ru (генеральный директор)</p>
                 </div>
                <h6 class="mt-3">Обратная связь</h6>
                <form>
                    <input type="text" id="cont_name" class="form-control mb-3 fbs" placeholder="Имя"> 
                    <input type="text" id="cont_phone" class="form-control mb-3 fbs" placeholder="Телефон">
                     <textarea id="cont_mess" class="form-control fbs mb-3" rows="4" placeholder="Сообщение..."></textarea> 
                    <button class="zak">Отправить</button>
                </form>
                </b-col>
            </b-row>
        
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
    .map{
        
        box-shadow: 2px 2px 8px 0px #00000036;
    }
    .item_inf{
        background: white;
        padding: 20px;
        border: 1px solid lightgrey;
        box-shadow: 2px 2px 8px 0px #00000036;
        
    }
    .b-icon{
        margin-right: 5px;
    }
    .fbs{
        box-shadow: 2px 2px 8px 0px #00000036;
    }
</style>