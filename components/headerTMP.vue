<template>
    <div class="header">
            <div class="wrapper">
                <div class="container">
                <img src="@/assets/imgs/Logo.png" alt="">
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
                    </div>
                </div>

                <div class="btn">
                    <span>
                        АВТОРИЗУЙТЕСЬ
                    </span>
                </div>
            </div>
        </div>
</template>


<style lang="scss" scoped>
@import "../assets/styles/main.scss";
.header{
    @include center;
    width: 100%;
    background: $main-bg;
    min-height: 65px;
    position: fixed;
    z-index: 5000;
    top: 0;
    left: 0;
    .wrapper{
        width: 90%;
        padding: 10px 0;
        @include center{
                justify-content: space-between;
        }
        .container{
            width: 100%;
            @include center{
               gap: 40px;
               justify-content: flex-start;
            }
        }
        .nav{
            display: flex;
            align-items: center;
            gap: 20px;
            a{
                text-decoration: none;
                @include h3;
            }
        }

        .btn{
            background: #FFFFFF;
            border-radius: 100px;
            width: 192px;
            height: 42px;
            @include center;
            span{
                @include h4{
                    font-weight: 500;
                }
            }
        }
    }

    @media (max-width:610px) {
        .wrapper .nav{
            display: none;
        }
    }
}
</style>