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
                         <nuxt-link v-if="user" to="/">
                           Отклики и предложения
                        </nuxt-link>
                    </div>
                </div>

                <div @click="auth=!auth" v-if="!user" class="btn">
                    <span>
                        АВТОРИЗУЙТЕСЬ
                    </span>
                </div>
                <div v-if="user" class="icons">
                    <img src="../assets/imgs/message.svg" alt="">
                    <img src="../assets/imgs/union.png" alt="">
                    <img src="../assets/imgs/notknow.png" alt="">
                </div>


                <img @click="profile=!profile" v-if="user" class="prof" src="../assets/imgs/profile.png" width="32" height="32" style="border-radius:50%;" alt="">


            </div>

            <transition name="slide-fade">
           <profile-modal v-if="profile"/>
            </transition>

            <transition name="slide-fade">
            <headerModal :user="user" v-if="isModal"/>
            </transition>


            <transition name="auth">
            <Modal v-if="auth" @close="auth=false" :mt="300">
              <component :is="authPage" @regis="regis" @login="login" @reset="reset" @send="page='send'"/>
            </Modal>
            </transition>


        </div>
</template>




<script>
import login from './auth/login.vue'
import Regis from './auth/register.vue'
import Reset from './auth/resetPassword.vue'
import send from './auth/send.vue'
import profileModal from './profile/profileModal.vue'
export default {
    data:()=>({
        isModal:false,
        auth:false,
        page:'login',
        profile:false,
        user:true
    }),
    computed:{
        authPage(){
            return this.page
            }
    },
    methods:{
        login(){
            this.page = 'login'
        },
        regis(){
            this.page = 'Regis'
        },
        reset(){
            this.page ='Reset'
        }

    },
    components:{
        login,
        Regis,
        Reset,
        send,
        profileModal
    }

}
</script>

<style lang="scss" scoped>
@import "../assets/styles/main.scss";
.prof{
    display: none;
}
.icons{
    display: flex;
    gap:10px;
    align-items: center;
}


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

.auth-enter-active {
  transition: all .3s ease;
}

.auth-enter, .auth-leave-to {
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
@media (max-width:1200px) {
    .icons{
        display: none;
    }
    .prof{
        display: block;
    }
}
</style>