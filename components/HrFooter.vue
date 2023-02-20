<template>
    <section class="footer">
        <div class="container">
            <b-container class="footer_block">
                <b-row>
                    <b-col>
                        <ul class="list-group">
                            <li>
                                <NuxtLink to="/o-kompanii" class="nav-link">О компании</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/allServices" class="nav-link">Все услуги</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/price" class="nav-link">Цены</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/informatsiya" class="nav-link">Информация</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/news" class="nav-link">Новости</NuxtLink>
                            </li>
                            <li> <a class="nav-link" href="#">Контакты</a></li>
                        </ul>
                    </b-col>
                    <b-col>
                        <ul class="list-group">
                            <li>Контактная информация:</li>
                            <li>
                                <b-icon icon="geo-alt-fill" style="color: #ee2738;"></b-icon>Москва, улица Ватутина, 11
                            </li>
                            <li>
                                <b-icon icon="geo-alt-fill" style="color: #ee2738;"></b-icon>Санкт Петербург, улица
                                Мытнинская, 12/44
                            </li>
                            <li>
                                <b-icon icon="telephone-fill" style="color: #ee2738;"></b-icon>+7 (495) 118-33-83
                            </li>
                            <li>
                                <a href="https://www.facebook.com/HR-Гарант-390447481428951/" target="_blank">
                                    <b-icon icon="facebook" style="color: #ffffff;"></b-icon>
                                </a>
                                <a href="https://www.youtube.com/channel/UC-65yu7DxH8ZCOVJEeY5DWg" target="_blank">
                                    <b-icon icon="youtube" style="color: #ffffff;"></b-icon>
                                </a>
                                <a href="https://vk.com/hrgarant" target="_blank">
                                    <b-img src="~/assets/images/vk.jpg"></b-img>
                                </a>
                            </li>
                            <li class="pt-2"><a href="tel:+74951183383">
                                    <b-button class="zak callme">Заказать звонок</b-button>
                                </a></li>
                        </ul>
                    </b-col>
                    <b-col>
                        <div style="position:relative;overflow:hidden;"><a
                                href="https://yandex.ru/maps/213/moscow/?utm_medium=mapframe&utm_source=maps"
                                style="color:#eee;font-size:12px;position:absolute;top:0px;">Москва</a><a
                                href="https://yandex.ru/maps/213/moscow/?from=api-maps&ll=37.453908%2C55.710731&mode=usermaps&origin=jsapi_2_1_78&um=constructor%3A195b64111e8becab6bc2c8f6aae91e509131e9a06c3f300348284a2792a703cb&utm_medium=mapframe&utm_source=maps&z=11"
                                style="color:#eee;font-size:12px;position:absolute;top:14px;">Яндекс.Карты — транспорт,
                                навигация, поиск
                                мест</a><iframe src="https://yandex.ru/map-widget/v1/-/CCUmy4RswA" width="450px"
                                height="250px" frameborder="1" allowfullscreen="true"
                                style="position:relative;"></iframe></div>
                    </b-col>
                </b-row>
            </b-container>
            <b-container class="footer-line">
                <b-row>
                    <b-col md-12>
                        <p class="ft">© 2004 — 2018 Московский кадровый центр «HR Гарант»</p>
                        <p class="ft">ОГРН 1127747250300 ИНН 7723857488</p>
                    </b-col>

                </b-row>
            </b-container>
        </div>
    </section>
</template>



<style scoped>
    .footer {
        background-image: url(~/assets/images/bg-footer.jpg);
        min-height: 300px;
    }

    .footer_block {
        padding-top: 25px;
        padding-bottom: 5px;
    }

    li {
        list-style-type: none;
        color: white;
    }

    a {
        color: white;

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
        text-decoration: none;


    }

    .footer-line {
        border-top: 1px solid rgba(255, 255, 255, 0.2);
        margin-top: 20px;
    }

    .ft {
        line-height: 1;
        text-align: center;
        color: white;
        font-size: 14px;
        margin-top: 5px;
    }
</style>