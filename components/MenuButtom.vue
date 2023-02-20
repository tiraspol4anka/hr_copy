<template>
    <section class="navbar_menu sticky-top">
        <b-navbar class="button_line" toggleable="lg" type="light">
            <b-navbar-brand></b-navbar-brand>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
            <b-collapse id="nav-collapse" is-nav>
                <b-container>
                    <n-link no-prefetch active to="/">
                        <img class="logo-icon" src="~/assets/images/logo2.svg" alt="" />
                    </n-link>
                    <b-navbar-nav>
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
                        <b-nav-item NuxtLink to="/kontakty">Контакты</NuxtLink>
                        </b-nav-item>
                    </b-navbar-nav>
                    <div>
                        <b-col class="phone">+7 (495) 118-33-83</b-col>
                        <b-col align="right"><a href="tel:+74951183383"><b-button class="zak callme">Заказать звонок</b-button></a>
                        </b-col>
                    </div>
                </b-container>
            </b-collapse>
        </b-navbar>
    </section>
</template>

<style scoped>
    .phone {
        font-size: 20px;
    }

    .button_line {
        box-shadow: 0 0 10px rgb(0 0 0 / 50%);
        background: rgb(253, 251, 251);
    }

    .logo-icon {
        width: 140px;
        margin-top: 10px;
        margin-bottom: 10px;
    }

    @media (max-width: 768px) {
        .logo-icon {
            display: none;
        }

        .navbar_menu {
            display: none;
        }
    }
</style>