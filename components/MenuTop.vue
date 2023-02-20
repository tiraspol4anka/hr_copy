<template>
    <b-container fluid class="bg-menu">
        <div class="container">
            <div class="top_line">
                <b-nav>
                    <b-nav-item>
                        <nuxt-link to=/autstaffing>Аутстаффинг</nuxt-link>
                    </b-nav-item>
                    <b-nav-item>
                        <nuxt-link to=/migratsionnyy-audit>Миграционный аудит</nuxt-link>
                    </b-nav-item>
                    <b-nav-item>
                        <nuxt-link to=/patent-na-rabotu>Патент на работу</nuxt-link>
                    </b-nav-item>
                    <b-nav-item>
                        <nuxt-link to=/seminary>Семинары</nuxt-link>
                    </b-nav-item>
                    <b-nav-item>
                        <nuxt-link to=/podbor-personala>Подбор персонала</nuxt-link>
                    </b-nav-item>
                    <b-nav-item>
                        <nuxt-link to=/snyatie-zapreta>Снятие запрета</nuxt-link>
                    </b-nav-item>
                    <b-nav-item>
                        <nuxt-link to=/goszakazchikam>Госзаказчикам</nuxt-link>
                    </b-nav-item>
                </b-nav>
            </div>
        </div>
    </b-container>
</template>
<style scoped>
    @media (max-width: 768px) {
        .top_line {
            display: none;
        }
    }

    .top_line {
        height: 40px;

    }

    .bg-menu {
        background: #313e49;
    }

    a {
        color: white;
        font-size: 14px;
        word-spacing: -1px;
        font-family: 'Roboto', sans-serif;

    }

    a:hover {
        text-decoration: none;
    }
</style>