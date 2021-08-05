<template>
    <div class="main">
        <div class="profile">
            <div class="profile-img-container">
                <div class="img">
                    <img src="../../assets/imgs/profile.png" alt="">
                </div>
                <svg width="24" height="23" viewBox="0 0 24 23" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M23.4353 8.94517L21.5907 8.5658C21.4303 8.1012 21.2316 7.64803 20.9971 7.2115L22.0182 5.70874C22.2006 5.44024 22.1605 5.08772 21.9221 4.86217L19.0485 2.14353C18.8101 1.91799 18.4374 1.88005 18.1536 2.05258L16.5652 3.01868C16.1038 2.79677 15.6248 2.60882 15.1337 2.45707L14.7327 0.711971C14.6611 0.40016 14.3692 0.177734 14.0319 0.177734H9.96808C9.6308 0.177734 9.33893 0.40016 9.26733 0.711971L8.86633 2.45707C8.37524 2.60882 7.89624 2.79677 7.43481 3.01868L5.84637 2.05258C5.56256 1.88005 5.18994 1.91799 4.95154 2.14353L2.07788 4.86217C1.83948 5.08772 1.79938 5.44024 1.98175 5.70874L3.00293 7.2115C2.76837 7.64803 2.5697 8.1012 2.4093 8.5658L0.564697 8.94517C0.235107 9.01307 0 9.28902 0 9.60811V13.4527C0 13.7718 0.235107 14.0478 0.564697 14.1157L2.4093 14.4951C2.5697 14.9597 2.76837 15.4128 3.00293 15.8494L1.98175 17.3521C1.79938 17.6206 1.83948 17.9731 2.07788 18.1987L4.95154 20.9173C5.18994 21.1429 5.56256 21.1808 5.84637 21.0083L7.43481 20.0422C7.89624 20.2641 8.37524 20.452 8.86633 20.6038L9.26733 22.3489C9.33893 22.6607 9.6308 22.8831 9.96808 22.8831H14.0319C14.3692 22.8831 14.6611 22.6607 14.7327 22.3489L15.1337 20.6038C15.6248 20.452 16.1038 20.2641 16.5652 20.0422L18.1536 21.0083C18.4374 21.1808 18.8101 21.143 19.0485 20.9173L21.9221 18.1987C22.1605 17.9731 22.2006 17.6206 22.0182 17.3521L20.9971 15.8494C21.2316 15.4128 21.4303 14.9597 21.5907 14.4951L23.4353 14.1157C23.7649 14.0478 24 13.7718 24 13.4527V9.60811C24 9.28902 23.7649 9.01307 23.4353 8.94517ZM16.3028 11.5304C16.3028 13.7749 14.3725 15.6011 12 15.6011C9.6275 15.6011 7.6972 13.7749 7.6972 11.5304C7.6972 9.28591 9.6275 7.45973 12 7.45973C14.3725 7.45973 16.3028 9.28591 16.3028 11.5304Z" fill="white"/>
                </svg>

            </div>

            <div class="full-name">
                Сергей Кроквин
            </div>
            <nuxt-link to="#">Редактировать профиль</nuxt-link>
        </div>
        <div class="settings-nav">
            <div class="title">Настройки</div>

            <div class="grid">
                <nuxt-link active-class="active-link" to="#" class="card">
                    <img src="../../assets/imgs/settings.png" alt="">
                    <div class="text">Профиль</div>
                </nuxt-link>
                <nuxt-link active-class="active-link" to="/profile/common-settings" class="card active-link">
                    <img src="../../assets/imgs/common-settings.png" alt="">
                    <div class="text">Общие</div>
                </nuxt-link>
                <nuxt-link active-class="active-link" to="/profile/job-subscription" class="card">
                    <img src="../../assets/imgs/follow.png" alt="">
                    <div class="text">Подписка 
                    на задания</div>
                </nuxt-link >
                <nuxt-link active-class="active-link" to="#" class="card">
                    <img src="../../assets/imgs/logout.png" alt="">
                    <div class="text">Выход</div>
                </nuxt-link>
            </div>
        </div>
        <div @click="$router.push('/profile/often-query')" class="often-query">
            <div class="title">Частые вопросы</div>
            <div class="queries">
                <div class="query">Сколько предложений я получу?</div>
                <div class="query">Обязательно ли выбирать исполнителя?</div>
                <div class="query"> Какую цену установить?</div>
                <div class="query">Как оплачивать услуги? </div>
                <div class="query">Как выбрать надежного исполнителя?</div>
                <div class="query">Как не выбрать исполнителем мошенника?</div>

            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
.main{
    width: 100%;
    @include center{
        flex-direction: column;
        gap:10px;
        justify-content: flex-start;
    }

    .often-query{
        width: 100%;
        padding: 50px 10px;
        background: #F9FAFF;
box-shadow: 1px 1px 25px rgba(136, 165, 191, 0.15);
border-radius: 6px;
        @include center{
        flex-direction: column;
        gap:10px;
        }
        .title{
            @include h2;

        }
        .queries{
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin: 20px 0;
        }
        .query{
            @include h4{
                color: $tg;
            }
        }
    }




    .settings-nav{
        background: #F9FAFF;
        box-shadow: 1px 1px 25px rgba(136, 165, 191, 0.15);
        border-radius: 6px;
        width: 100%;
        padding: 51px 35px;
         @include center{
        flex-direction: column;
        gap:10px;
        }
    
        .grid{
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-gap: 20px;
            margin: 20px 0;
            a{
                text-decoration: none;
            }
        }
        .card{
           @include center{
        flex-direction: column;
        gap:10px;
        width: 122px;
        height: 92px;
        }
        background: #F9FAFF;
        box-shadow: 2px 3px 7px rgba(136, 165, 191, 0.48), -2px -2px 10px #FFFFFF, inset 2px 1px 2px rgba(255, 255, 255, 0.4);
        border-radius: 8px;
        .text{
            @include h4{
                color: #4097E3;
                text-align: center;
            }
        } 
        }
        .title{
            @include h2;
        }

    }
    .active-link{
       box-shadow: inset -2px -2px 4px #FFFFFF, inset 2px 2px 2px rgba(136, 165, 191, 0.48);
    }

    .profile{
        margin: 0 0 40px 0;
       @include center{
        flex-direction: column;
        gap:10px;
        .full-name{
            @include h2;
        }
        a{
            @include h4;
        }



        .profile-img-container{
            position: relative;

            .img{
                border-radius: 50%;
            }

            svg{
                position: absolute;
                right: 0;
                bottom: 0;
            }
        }
    }  
    }
}

@media (max-width:1200px) {
    .main{

        display: none;
    }
 
}
</style>