<template>
    <div class="header">
            <div class="wrapper">
                <div class="container">
                    <div @click="isModal=!isModal" class="burger">
                        <div class="bline" :class="{active:isModal}"></div>
                        <div class="bline" :class="{active:isModal}"></div>
                        <div class="bline" :class="{active:isModal}"></div>
                    </div>
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
            <transition name="slide-fade">
            <headerModal v-if="isModal"/>
            </transition>
        </div>
</template>

<script>
export default {
    data:()=>({
        isModal:false
    })
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/main.scss";
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active до версии 2.1.8 */ {
  transform: translateX(- 30vw);
  opacity: 0;
}
.header{
    @include center;
    width: 100%;
    background: $main-bg;
    min-height: 65px;
    position: fixed;
    z-index: 5000;
    top: 0;
    left: 0;
    .burger{
        display: none;
    }
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
        .burger{
            display: flex;
            flex-direction: column;
            gap:5px;
            .bline{
                width: 30px ;
                height: 5px;
                background: #fff;
            }
            .active:nth-child(1){
                transition: all .9s ease;
                position: absolute;
                top: 30px;
                left: 25px;
                transform: rotate(45deg);
            }
            .active:nth-child(2){
                transition: all .9s ease;
                position: absolute;
                top: 30px;
                left: 25px;
                transform: rotate(- 45deg);
            }
            .active:nth-child(3){
               display: none;
            }
        }
    }
}
</style>