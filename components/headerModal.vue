<template>
    <div class="main">
         <div class="nav">
                        <nuxt-link to="/">
                    Создать задание
                        </nuxt-link>
                        <nuxt-link to="/">
                            Найти задание
                        </nuxt-link>
                        <nuxt-link to="/">
                            Исполнители
                        </nuxt-link>
                         <nuxt-link v-if="user" to="/">
                            Отклики и предложения
                        </nuxt-link>

        </div>
    </div>
</template>

<script>
export default {
    props:['user']
}
</script>


<style lang="scss" scoped>
@import "../assets/styles/main.scss";
.main{
    position: fixed;
    top: 65px;
    left: 0;
    width: 100%;
    z-index: 4000;
    min-height: calc(100vh - 65px);
    background: #fff;
    backdrop-filter: blur(10px);
    @include center;
    .nav{
        width: 90%;
        @include center{
            flex-direction: column;
            gap: 20px;
        }
        a{
            @include h2;
            text-decoration: none;
        }
    }
}
</style>