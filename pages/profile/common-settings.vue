<template>
    <div class="main-common">
        <div class="container-common">
             <div class="title">Общие настройки</div>
        <div class="flex">
            <div class="text">Имя</div>
            <input type="text">
        </div>
         <div class="flex">
            <div class="text">Фамилия</div>
            <input type="text">
        </div>

        <div class="flex">
            <div class="text">Дата рождения</div>
            <input type="date">
        </div>
        <div class="fl">
            <div class="text">Пол</div>
               <div>
                <input class="rad" type="radio" name="rb" id="rb2"> <label for="rb2">Муж.</label>
                </div>
                <div>
                <input class="rad"  type="radio" name="rb" id="rb3"> <label for="rb3">Жен.</label>
                </div>
        </div>


        <div class="flex" style="margin-top:120px;">
            <div class="text">Телефон</div>
            <input type="text">
             <div class="swic">
                       <switch-1 />
                       <span>Скрыть от других пользователей</span>
                </div>
        </div>
         <div class="flex">
            <div class="text">Е-mail</div>
            <input type="text">
             <div class="swic">
                       <switch-1 />
                       <span>Скрыть от других пользователей</span>
                </div>
        </div>
        <div class="flex">
            <div class="text">Vkontakte</div>
            <input type="text">
            <div class="swic">
                       <switch-1 />
                       <span>Скрыть от других пользователей</span>
                </div>
        </div>
         <div class="flex">
            <div class="text">Facebook</div>
            <input type="text">
            <div class="swic">
                       <switch-1 />
                       <span>Скрыть от других пользователей</span>
                </div>
        </div>
        <div class="flex">
            <div class="text">Instagram</div>
            <input type="text">
            <div class="swic">
                       <switch-1 />
                       <span>Скрыть от других пользователей</span>
                </div>
        </div>
        <div class="flex">
            <div class="text"></div>
        <div class="btn-blue" style="margin-left:5px">
            <span>СОХРАНИТЬ</span>
        </div>
        </div>




        </div>
        <div class="container-common">
            <div class="title">Изменить пароль</div>
                <div class="flex">
                    <div class="text">Старый пароль</div>
                    <div class="password">
                        <input show="false" :type="show1" >

                         <svg v-if="show1=='password'" @click="show1='text'" width="18" height="6" viewBox="0 0 18 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.0447 1.0515L17.174 0.969172C17.4257 0.801214 17.4849 0.469603 17.3107 0.228352C17.1349 -0.0150493 16.7893 -0.0699825 16.5428 0.0956798C7.91817 5.91294 1.64006 0.381967 1.37632 0.144302C1.15376 -0.0566439 0.803042 -0.0464608 0.595794 0.166964C0.387505 0.381249 0.397615 0.716448 0.617946 0.918111C0.62984 0.929012 0.826235 1.10242 1.18468 1.35902L0.0799033 3.11676C-0.0776886 3.36747 0.00497264 3.69478 0.264999 3.84811C0.353905 3.89974 0.454853 3.92571 0.55253 3.92571C0.738221 3.92571 0.919006 3.83463 1.02412 3.67069L2.10437 1.95339C2.71005 2.3091 3.48671 2.69751 4.41205 3.02568L3.87965 4.74283C3.79149 5.02553 3.95637 5.32043 4.24762 5.40448L4.4064 5.42714C4.64174 5.42714 4.86178 5.27797 4.93344 5.04719L5.46063 3.35356C6.31475 3.57889 7.27026 3.73107 8.30145 3.76722V5.46802C8.30145 5.76234 8.5478 6 8.85287 6C9.15765 6 9.40415 5.76234 9.40415 5.46802V3.75775C10.3039 3.71013 11.2575 3.56082 12.2531 3.28687L12.9318 5.01348C13.0164 5.22619 13.226 5.35643 13.4474 5.35643L13.6425 5.32286C13.9272 5.21845 14.0715 4.91165 13.9633 4.63712L13.3025 2.95482C14.2091 2.62995 15.1461 2.20224 16.114 1.63483L17.0074 2.78529C17.1162 2.92427 17.2823 2.99886 17.4482 2.99886C17.5638 2.99886 17.6794 2.96501 17.7785 2.892C18.0229 2.71558 18.0723 2.38211 17.8903 2.14731L17.0447 1.0515Z" fill="#D6E4F0"/>
                        </svg>

                        <svg  @click="show1='password'" v-else width="18" height="12" viewBox="0 0 18 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.8856 5.6338C17.7248 5.40371 13.8934 0 8.99992 0C4.10647 0 0.274852 5.40371 0.114223 5.63358C-0.0380743 5.85186 -0.0380743 6.14792 0.114223 6.3662C0.274852 6.59629 4.10647 12 8.99992 12C13.8934 12 17.7248 6.59625 17.8856 6.36638C18.0381 6.14814 18.0381 5.85186 17.8856 5.6338ZM8.99992 10.7586C5.39538 10.7586 2.27346 7.17207 1.3493 5.99958C2.27226 4.82605 5.38764 1.24137 8.99992 1.24137C12.6043 1.24137 15.726 4.8273 16.6505 6.00042C15.7276 7.17391 12.6122 10.7586 8.99992 10.7586Z" fill="#4097E3"/>
                        <path d="M9.00003 2.27539C7.03683 2.27539 5.43958 3.94608 5.43958 5.99954C5.43958 8.053 7.03683 9.72369 9.00003 9.72369C10.9632 9.72369 12.5605 8.053 12.5605 5.99954C12.5605 3.94608 10.9632 2.27539 9.00003 2.27539ZM9.00003 8.48229C7.69116 8.48229 6.62642 7.36855 6.62642 5.99954C6.62642 4.63053 7.6912 3.5168 9.00003 3.5168C10.3089 3.5168 11.3736 4.63053 11.3736 5.99954C11.3736 7.36855 10.3089 8.48229 9.00003 8.48229Z" fill="#4097E3"/>
                        </svg>

                    </div>
                 </div>

                  <div class="flex">
                    <div class="text">Новый пароль</div>
                    <div class="password">
                        <input show="false" :type="show2" >

                         <svg v-if="show2=='password'" @click="show2='text'" width="18" height="6" viewBox="0 0 18 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.0447 1.0515L17.174 0.969172C17.4257 0.801214 17.4849 0.469603 17.3107 0.228352C17.1349 -0.0150493 16.7893 -0.0699825 16.5428 0.0956798C7.91817 5.91294 1.64006 0.381967 1.37632 0.144302C1.15376 -0.0566439 0.803042 -0.0464608 0.595794 0.166964C0.387505 0.381249 0.397615 0.716448 0.617946 0.918111C0.62984 0.929012 0.826235 1.10242 1.18468 1.35902L0.0799033 3.11676C-0.0776886 3.36747 0.00497264 3.69478 0.264999 3.84811C0.353905 3.89974 0.454853 3.92571 0.55253 3.92571C0.738221 3.92571 0.919006 3.83463 1.02412 3.67069L2.10437 1.95339C2.71005 2.3091 3.48671 2.69751 4.41205 3.02568L3.87965 4.74283C3.79149 5.02553 3.95637 5.32043 4.24762 5.40448L4.4064 5.42714C4.64174 5.42714 4.86178 5.27797 4.93344 5.04719L5.46063 3.35356C6.31475 3.57889 7.27026 3.73107 8.30145 3.76722V5.46802C8.30145 5.76234 8.5478 6 8.85287 6C9.15765 6 9.40415 5.76234 9.40415 5.46802V3.75775C10.3039 3.71013 11.2575 3.56082 12.2531 3.28687L12.9318 5.01348C13.0164 5.22619 13.226 5.35643 13.4474 5.35643L13.6425 5.32286C13.9272 5.21845 14.0715 4.91165 13.9633 4.63712L13.3025 2.95482C14.2091 2.62995 15.1461 2.20224 16.114 1.63483L17.0074 2.78529C17.1162 2.92427 17.2823 2.99886 17.4482 2.99886C17.5638 2.99886 17.6794 2.96501 17.7785 2.892C18.0229 2.71558 18.0723 2.38211 17.8903 2.14731L17.0447 1.0515Z" fill="#D6E4F0"/>
                        </svg>

                        <svg  @click="show2='password'" v-else width="18" height="12" viewBox="0 0 18 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.8856 5.6338C17.7248 5.40371 13.8934 0 8.99992 0C4.10647 0 0.274852 5.40371 0.114223 5.63358C-0.0380743 5.85186 -0.0380743 6.14792 0.114223 6.3662C0.274852 6.59629 4.10647 12 8.99992 12C13.8934 12 17.7248 6.59625 17.8856 6.36638C18.0381 6.14814 18.0381 5.85186 17.8856 5.6338ZM8.99992 10.7586C5.39538 10.7586 2.27346 7.17207 1.3493 5.99958C2.27226 4.82605 5.38764 1.24137 8.99992 1.24137C12.6043 1.24137 15.726 4.8273 16.6505 6.00042C15.7276 7.17391 12.6122 10.7586 8.99992 10.7586Z" fill="#4097E3"/>
                        <path d="M9.00003 2.27539C7.03683 2.27539 5.43958 3.94608 5.43958 5.99954C5.43958 8.053 7.03683 9.72369 9.00003 9.72369C10.9632 9.72369 12.5605 8.053 12.5605 5.99954C12.5605 3.94608 10.9632 2.27539 9.00003 2.27539ZM9.00003 8.48229C7.69116 8.48229 6.62642 7.36855 6.62642 5.99954C6.62642 4.63053 7.6912 3.5168 9.00003 3.5168C10.3089 3.5168 11.3736 4.63053 11.3736 5.99954C11.3736 7.36855 10.3089 8.48229 9.00003 8.48229Z" fill="#4097E3"/>
                        </svg>

                    </div>
                 </div>

                  <div class="flex">
                    <div class="text">Повторите пароль</div>
                    <div class="password">
                        <input show="false" :type="show3" >

                         <svg v-if="show3=='password'" @click="show3='text'" width="18" height="6" viewBox="0 0 18 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.0447 1.0515L17.174 0.969172C17.4257 0.801214 17.4849 0.469603 17.3107 0.228352C17.1349 -0.0150493 16.7893 -0.0699825 16.5428 0.0956798C7.91817 5.91294 1.64006 0.381967 1.37632 0.144302C1.15376 -0.0566439 0.803042 -0.0464608 0.595794 0.166964C0.387505 0.381249 0.397615 0.716448 0.617946 0.918111C0.62984 0.929012 0.826235 1.10242 1.18468 1.35902L0.0799033 3.11676C-0.0776886 3.36747 0.00497264 3.69478 0.264999 3.84811C0.353905 3.89974 0.454853 3.92571 0.55253 3.92571C0.738221 3.92571 0.919006 3.83463 1.02412 3.67069L2.10437 1.95339C2.71005 2.3091 3.48671 2.69751 4.41205 3.02568L3.87965 4.74283C3.79149 5.02553 3.95637 5.32043 4.24762 5.40448L4.4064 5.42714C4.64174 5.42714 4.86178 5.27797 4.93344 5.04719L5.46063 3.35356C6.31475 3.57889 7.27026 3.73107 8.30145 3.76722V5.46802C8.30145 5.76234 8.5478 6 8.85287 6C9.15765 6 9.40415 5.76234 9.40415 5.46802V3.75775C10.3039 3.71013 11.2575 3.56082 12.2531 3.28687L12.9318 5.01348C13.0164 5.22619 13.226 5.35643 13.4474 5.35643L13.6425 5.32286C13.9272 5.21845 14.0715 4.91165 13.9633 4.63712L13.3025 2.95482C14.2091 2.62995 15.1461 2.20224 16.114 1.63483L17.0074 2.78529C17.1162 2.92427 17.2823 2.99886 17.4482 2.99886C17.5638 2.99886 17.6794 2.96501 17.7785 2.892C18.0229 2.71558 18.0723 2.38211 17.8903 2.14731L17.0447 1.0515Z" fill="#D6E4F0"/>
                        </svg>

                        <svg  @click="show3='password'" v-else width="18" height="12" viewBox="0 0 18 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.8856 5.6338C17.7248 5.40371 13.8934 0 8.99992 0C4.10647 0 0.274852 5.40371 0.114223 5.63358C-0.0380743 5.85186 -0.0380743 6.14792 0.114223 6.3662C0.274852 6.59629 4.10647 12 8.99992 12C13.8934 12 17.7248 6.59625 17.8856 6.36638C18.0381 6.14814 18.0381 5.85186 17.8856 5.6338ZM8.99992 10.7586C5.39538 10.7586 2.27346 7.17207 1.3493 5.99958C2.27226 4.82605 5.38764 1.24137 8.99992 1.24137C12.6043 1.24137 15.726 4.8273 16.6505 6.00042C15.7276 7.17391 12.6122 10.7586 8.99992 10.7586Z" fill="#4097E3"/>
                        <path d="M9.00003 2.27539C7.03683 2.27539 5.43958 3.94608 5.43958 5.99954C5.43958 8.053 7.03683 9.72369 9.00003 9.72369C10.9632 9.72369 12.5605 8.053 12.5605 5.99954C12.5605 3.94608 10.9632 2.27539 9.00003 2.27539ZM9.00003 8.48229C7.69116 8.48229 6.62642 7.36855 6.62642 5.99954C6.62642 4.63053 7.6912 3.5168 9.00003 3.5168C10.3089 3.5168 11.3736 4.63053 11.3736 5.99954C11.3736 7.36855 10.3089 8.48229 9.00003 8.48229Z" fill="#4097E3"/>
                        </svg>

                    </div>
                 </div>
                <div class="flex">
                <div class="text"></div>
                <div class="btn-blue" style="margin-left:5px">
                <span>СОХРАНИТЬ</span>
                </div>
                </div>
        </div>

        <div class="container-common">
              <div class="title">Уведомления</div>
               <div class="flex">
                <div class="text">E-mail</div>
                <input type="text">
                <div class="swic">
                       <switch-1 />
                       <span>Получать на почту указанную в визитке</span>
                </div>
            </div>
            <div class="flex">
                <div class="text"></div>
                <div class="btn-blue" style="margin-left:5px">
                <span>СОХРАНИТЬ</span>
                </div>
                </div>

                <div class="flex">
                <div class="text" >
                </div>
                <nuxt-link to="#">Удалить профиль</nuxt-link>
                </div>
        </div>
    </div>
</template>

<script>
import Switch1 from '../../components/switch.vue'


export default {
    data:()=>({
        show1:'password',
        show2:'password',
        show3:'password',


    }),
    components:{
        Switch1
    
    }

}
</script>


<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
.btn-blue
{
    @include btn-blue;
}

.swic {
display: flex;
margin: 0 0 0 30px;
gap :20px;
justify-content: space-between;
align-items: center;
  & > span{
       width: 152px;
      color: #8CA2B7;
        font-size: 14px;
        line-height: 21px;
  }
}



 .password{
        width: 254px;
        height: 33px;
        @include center;
        background: #F4F9FE;
        box-shadow: inset 2px 2px 3px rgba(136, 165, 191, 0.48);
        border-radius: 20px;
        padding: 0 10px;
        &>input{
            width: 90%;
            height: 43px;
            background: transparent;
            border:none;
            outline: none;
            text-align: center;
        } 
    }
input:not([show=false]){
    background: #F4F9FE;
box-shadow: inset 2px 2px 3px rgba(136, 165, 191, 0.48);
border-radius: 20px;
width: 254px;
height: 33px;
border:none;
outline: none;
text-align: center;
padding: 2px 10px;
}
.main-common{
    width: 100%;
    .container-common{
        width: 100%;
        padding: 30px 0 0 90px;
        .title{
            @include h2;
            margin: 0 0 60px 0;
        }
    }

    .title{
        @include h2{
            text-align: center;
        }
    }
    .flex,.fl{
        display: flex;
        align-items: center;
        margin: 21px;
        .text{
            width: 200px;
            @include h4{
                color:$tg;
            }
        }
       
        a{
            @include h4{
                color: rgba(61, 149, 226, 1);
                text-align: center;
                margin-left: 10%;
                margin-top: 100px;
            }
        }
    }
    @media (max-width:1200px) {
        .container-common{
            padding: 30px 0 0 0px;
        }
    }

    @media (max-width:905px) {
        .flex{
            flex-direction: column;
        }
        .fl{
            @include center;
        }
        .fl .text{
            width:70px;
        }
    }

    @media (max-width:312px) {
        .flex{
            margin: 30px 0;
        }
    }
    
}


.rad:checked, 
.rad:not(:checked) 
{
    position: absolute;
    left: -9999px;
}

.rad:checked + label, 
.rad:not(:checked) + label {
    display: inline-block;
    position: relative;
    padding-left: 28px;
    line-height: 20px;
    padding-right: 20px;
    cursor: pointer;
}
.rad:checked + label:before, 
.rad:not(:checked) + label:before {
    content: "";
    position: absolute;
    left: 0px;
    top: 0px;
    width: 18px;
    height: 18px;
    border: 1px solid #dddddd;
    background-color: #ffffff;
}



.rad:checked + label:before, 
.rad:not(:checked) + label:before {
    &:nth-child(2){
        margin-left: 20px;
    }
    border-radius: 100%;
    
}

.rad:checked + label:after, 
.rad:not(:checked) + label:after {
    content: "";
    position: absolute;
    -webkit-transition: all 0.2s ease;
    -moz-transition: all 0.2s ease;
    -o-transition: all 0.2s ease;
    transition: all 0.2s ease;
}



.rad:checked + label:after, 
.rad:not(:checked) + label:after {
    left: 5px;
    top: 5px;
    width: 10px;
    height: 10px;
    border-radius: 100%;
    background-color: #4097E3;
}
 
.rad:not(:checked) + label:after {
    opacity: 0;
}
 
.rad:checked + label:after {
    opacity: 1;
}
.rad:nth-child(2){
    margin-left: 200px;
}

label{
    @include h4{
        color: $tg;
    }
}


</style>