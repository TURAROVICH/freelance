<template>
    <div class="container-modal">
                    <div class="title">
                        Регистрация
                    </div>
                    <div class="des">Войти через:</div>
                    <div class="icons">
                        <img src="../../assets/imgs/google.png" alt="">
                        <img src="../../assets/imgs/vk.png" alt="">
                        <img src="../../assets/imgs/fb.png" alt="">

                    </div>
                    <input placeholder="Имя"/>
                    <div class="password">
                        <input show="false" :type="show1" placeholder="Пароль">

                        <svg v-if="show1=='password'" @click="show1='text'" width="18" height="6" viewBox="0 0 18 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.0447 1.0515L17.174 0.969172C17.4257 0.801214 17.4849 0.469603 17.3107 0.228352C17.1349 -0.0150493 16.7893 -0.0699825 16.5428 0.0956798C7.91817 5.91294 1.64006 0.381967 1.37632 0.144302C1.15376 -0.0566439 0.803042 -0.0464608 0.595794 0.166964C0.387505 0.381249 0.397615 0.716448 0.617946 0.918111C0.62984 0.929012 0.826235 1.10242 1.18468 1.35902L0.0799033 3.11676C-0.0776886 3.36747 0.00497264 3.69478 0.264999 3.84811C0.353905 3.89974 0.454853 3.92571 0.55253 3.92571C0.738221 3.92571 0.919006 3.83463 1.02412 3.67069L2.10437 1.95339C2.71005 2.3091 3.48671 2.69751 4.41205 3.02568L3.87965 4.74283C3.79149 5.02553 3.95637 5.32043 4.24762 5.40448L4.4064 5.42714C4.64174 5.42714 4.86178 5.27797 4.93344 5.04719L5.46063 3.35356C6.31475 3.57889 7.27026 3.73107 8.30145 3.76722V5.46802C8.30145 5.76234 8.5478 6 8.85287 6C9.15765 6 9.40415 5.76234 9.40415 5.46802V3.75775C10.3039 3.71013 11.2575 3.56082 12.2531 3.28687L12.9318 5.01348C13.0164 5.22619 13.226 5.35643 13.4474 5.35643L13.6425 5.32286C13.9272 5.21845 14.0715 4.91165 13.9633 4.63712L13.3025 2.95482C14.2091 2.62995 15.1461 2.20224 16.114 1.63483L17.0074 2.78529C17.1162 2.92427 17.2823 2.99886 17.4482 2.99886C17.5638 2.99886 17.6794 2.96501 17.7785 2.892C18.0229 2.71558 18.0723 2.38211 17.8903 2.14731L17.0447 1.0515Z" fill="#D6E4F0"/>
                        </svg>

                        <svg  @click="show1='password'" v-else width="18" height="12" viewBox="0 0 18 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.8856 5.6338C17.7248 5.40371 13.8934 0 8.99992 0C4.10647 0 0.274852 5.40371 0.114223 5.63358C-0.0380743 5.85186 -0.0380743 6.14792 0.114223 6.3662C0.274852 6.59629 4.10647 12 8.99992 12C13.8934 12 17.7248 6.59625 17.8856 6.36638C18.0381 6.14814 18.0381 5.85186 17.8856 5.6338ZM8.99992 10.7586C5.39538 10.7586 2.27346 7.17207 1.3493 5.99958C2.27226 4.82605 5.38764 1.24137 8.99992 1.24137C12.6043 1.24137 15.726 4.8273 16.6505 6.00042C15.7276 7.17391 12.6122 10.7586 8.99992 10.7586Z" fill="#4097E3"/>
                        <path d="M9.00003 2.27539C7.03683 2.27539 5.43958 3.94608 5.43958 5.99954C5.43958 8.053 7.03683 9.72369 9.00003 9.72369C10.9632 9.72369 12.5605 8.053 12.5605 5.99954C12.5605 3.94608 10.9632 2.27539 9.00003 2.27539ZM9.00003 8.48229C7.69116 8.48229 6.62642 7.36855 6.62642 5.99954C6.62642 4.63053 7.6912 3.5168 9.00003 3.5168C10.3089 3.5168 11.3736 4.63053 11.3736 5.99954C11.3736 7.36855 10.3089 8.48229 9.00003 8.48229Z" fill="#4097E3"/>
                        </svg>

                    </div>
                    <div class="password">
                        <input show="false" :type="show2" placeholder="Пароль">

                         <svg v-if="show2=='password'" @click="show2='text'" width="18" height="6" viewBox="0 0 18 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.0447 1.0515L17.174 0.969172C17.4257 0.801214 17.4849 0.469603 17.3107 0.228352C17.1349 -0.0150493 16.7893 -0.0699825 16.5428 0.0956798C7.91817 5.91294 1.64006 0.381967 1.37632 0.144302C1.15376 -0.0566439 0.803042 -0.0464608 0.595794 0.166964C0.387505 0.381249 0.397615 0.716448 0.617946 0.918111C0.62984 0.929012 0.826235 1.10242 1.18468 1.35902L0.0799033 3.11676C-0.0776886 3.36747 0.00497264 3.69478 0.264999 3.84811C0.353905 3.89974 0.454853 3.92571 0.55253 3.92571C0.738221 3.92571 0.919006 3.83463 1.02412 3.67069L2.10437 1.95339C2.71005 2.3091 3.48671 2.69751 4.41205 3.02568L3.87965 4.74283C3.79149 5.02553 3.95637 5.32043 4.24762 5.40448L4.4064 5.42714C4.64174 5.42714 4.86178 5.27797 4.93344 5.04719L5.46063 3.35356C6.31475 3.57889 7.27026 3.73107 8.30145 3.76722V5.46802C8.30145 5.76234 8.5478 6 8.85287 6C9.15765 6 9.40415 5.76234 9.40415 5.46802V3.75775C10.3039 3.71013 11.2575 3.56082 12.2531 3.28687L12.9318 5.01348C13.0164 5.22619 13.226 5.35643 13.4474 5.35643L13.6425 5.32286C13.9272 5.21845 14.0715 4.91165 13.9633 4.63712L13.3025 2.95482C14.2091 2.62995 15.1461 2.20224 16.114 1.63483L17.0074 2.78529C17.1162 2.92427 17.2823 2.99886 17.4482 2.99886C17.5638 2.99886 17.6794 2.96501 17.7785 2.892C18.0229 2.71558 18.0723 2.38211 17.8903 2.14731L17.0447 1.0515Z" fill="#D6E4F0"/>
                        </svg>

                        <svg  @click="show2='password'" v-else width="18" height="12" viewBox="0 0 18 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.8856 5.6338C17.7248 5.40371 13.8934 0 8.99992 0C4.10647 0 0.274852 5.40371 0.114223 5.63358C-0.0380743 5.85186 -0.0380743 6.14792 0.114223 6.3662C0.274852 6.59629 4.10647 12 8.99992 12C13.8934 12 17.7248 6.59625 17.8856 6.36638C18.0381 6.14814 18.0381 5.85186 17.8856 5.6338ZM8.99992 10.7586C5.39538 10.7586 2.27346 7.17207 1.3493 5.99958C2.27226 4.82605 5.38764 1.24137 8.99992 1.24137C12.6043 1.24137 15.726 4.8273 16.6505 6.00042C15.7276 7.17391 12.6122 10.7586 8.99992 10.7586Z" fill="#4097E3"/>
                        <path d="M9.00003 2.27539C7.03683 2.27539 5.43958 3.94608 5.43958 5.99954C5.43958 8.053 7.03683 9.72369 9.00003 9.72369C10.9632 9.72369 12.5605 8.053 12.5605 5.99954C12.5605 3.94608 10.9632 2.27539 9.00003 2.27539ZM9.00003 8.48229C7.69116 8.48229 6.62642 7.36855 6.62642 5.99954C6.62642 4.63053 7.6912 3.5168 9.00003 3.5168C10.3089 3.5168 11.3736 4.63053 11.3736 5.99954C11.3736 7.36855 10.3089 8.48229 9.00003 8.48229Z" fill="#4097E3"/>
                        </svg>

                    </div>
                     <input type="text" placeholder="E-mail">

                            <label class="container-c">Принимаю условия <nuxt-link to="#">соглашения</nuxt-link>
                            <input type="checkbox">
                            <span class="checkmark"></span>
                            </label>

                    <div class="btn">
                        <span>Регистрация</span>
                    </div>
                     <span @click="$emit('login')" class="l">Войти</span>

                </div>
</template>

<script>
export default {
    data:()=>({
        show1:'password',
        show2:'password'
    })
}
</script>


<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
@import '../../assets/styles/auth.scss';


.container-c {
  display: block;
  position: relative;
  padding-left: 35px;
  margin-bottom: 12px;
  cursor: pointer;
  @include h4;
  a{
   @include h4 
  }
  @include center;
  gap  :5px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* Hide the browser's default checkbox */
.container-c input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
}

/* Create a custom checkbox */
.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 25px;
  width: 25px;
  background: #F9FAFF;
box-shadow: inset -2px -2px 4px #FFFFFF, inset 2px 2px 2px rgba(136, 165, 191, 0.48);
border-radius: 2px;
}

/* On mouse-over, add a grey background color */
.container-c:hover input ~ .checkmark {
   background: #F9FAFF;
box-shadow: inset -2px -2px 4px #FFFFFF, inset 2px 2px 2px rgba(136, 165, 191, 0.48);
border-radius: 2px;
}

/* When the checkbox is checked, add a blue background */
.container-c input:checked ~ .checkmark {
  background-color: #fff;
}

/* Create the checkmark/indicator (hidden when not checked) */
.checkmark:after {
  content: "";
  position: absolute;
  display: none;
}

/* Show the checkmark when checked */
.container-c input:checked ~ .checkmark:after {
  display: block;
}

/* Style the checkmark/indicator */
.container-c .checkmark:after {
  left: 9px;
  top: 5px;
  width: 5px;
  height: 10px;
  border: solid  #31456A;
  border-width: 0 3px 3px 0;
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
}
</style>