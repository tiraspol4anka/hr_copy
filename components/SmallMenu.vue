<template>
    <section class="navbar_menu sticky-top" style="display: block;">
        <b-navbar toggleable="sm" type="light">
            <b-navbar-brand></b-navbar-brand>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
            <b-collapse id="nav-collapse" is-nav>
                <b-container>
                    <b-navbar-nav class="smenu">
                        <b-nav-item NuxtLink to="/o-kompanii">О компании</NuxtLink>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/allServices">Все услуги</NuxtLink>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/price">Цены</NuxtLink>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/informatsiya">Информация</NuxtLink>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/news">Новости</NuxtLink>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/price">Контакты</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/autstaffing">Аутстаффинг</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/migratsionnyy-audit">Миграционный аудит</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/patent-na-rabotu">Патент на работу</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/seminary">Семинары</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/podbor-personala">Подбор персонала</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/snyatie-zapreta">Снятие запрета</NuxtLink>
                        </b-nav-item>
                        </b-nav-item>
                        <b-nav-item NuxtLink to="/goszakazchikam">Госзаказчикам</NuxtLink>
                        </b-nav-item>
                    </b-navbar-nav>
                </b-container>
            </b-collapse>
        </b-navbar>
    </section>
</template>

<style scoped>
    .navbar_menu {
        z-index: 9999;

        right: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background-color: transparent;


    }

    .smenu {
        background: url("~/assets/images/slide-2-img.jpg");
        background-size: cover;
        height: 100%;
        width: 100%;
        top: 0;
        left: 0;
        position: fixed;
        z-index: 9999;
    }

    .navbar-light .navbar-nav .nav-link {
        color: #f8f9fa;
        text-align: center;
        border-bottom: 1px solid #d8d8d8;
    }

    .navbar-nav {
        padding-left: 20px;
        padding-right: 20px;
        padding-top: 40px;
    }

    @media screen and (max-width: 768px) {
        .logo-icon {
            display: none;
        }



    }
    .logo-icon {
        width: 140px;
        margin-top: 10px;
        margin-bottom: 10px;
    }

    @media screen and (min-width: 768px) {
        .navbar {
            display: none;
        }
    }
</style>