<template>
  <div class="main">
     <div class="wrapper">
          <div class="welcome-part">
            <img class="main-img" src="../assets/imgs/welcome-part.png" alt="">
            <img src="../assets/imgs/ura.png" class="abs" alt="">
            <img class="shadow" src="../assets/imgs/shadow.png" alt="">
            <div class="content">
              <img src="../assets/imgs/el.png" alt="">
              <div class="title">
                Организуй праздник сам!
              </div>
              <div class="des">
                Найди проверенных людей для своего праздника
              </div>

              <div class="btns">
                <div class="btn"><span>СОЗДАТЬ ЗАДАНИЕ</span></div>
                <div class="link"><nuxt-link to="#">Смотреть предложения</nuxt-link></div>
              </div>
            </div>
          </div>


          <div class="about-part">
              <div class="title">
Еasyfest дает возможность сэкономить время 
для организации Вашего незабываемого праздника
              </div>
              <div class="des">
Для Вас мы стараемся  тщательно отбирать надежных и проверенных исполнителей. Ежедневно отслеживая недобросовестных и некомпетентных поставщиков услуг.  Нам Вы можете легко доверить любой Ваш праздник.
              </div>
          </div>

          <div class="spezialition">
            <img src="../assets/imgs/spez.svg" alt="">


            <div class="container">
                <div class="title">Специализации</div>

                <div class="links">
                    <div class="link">
                      <div class="title">Декор, инвентарь </div>
                    <ul>
                      <li>Шарики </li>
                      <li>Флористика </li>
                      <li>Декор </li>
                      <li>Транспорт</li>
                    </ul>
                    </div>

                    <div class="link">
                      <div class="title">Персонал  </div>
                    <ul>
                      <li>Ведущие  </li>
                      <li>Аниматоры  </li>
                      <li>Фото/видеосъемка  </li>
                      <li>Артисты</li>
                       <li>Стилисты</li>
                    </ul>
                    </div>


                    <div class="link">
                      <div class="title">Площадки </div>
                    <ul>
                      <li>Рестораны  </li>
                      <li>Кафе </li>
                      <li>Банкетные залы  </li>
                      <li>Кейтеринг</li>
                      <li>Детские площадки</li>
                    </ul>
                    </div>

                    <div class="link">
                      <div class="title">Праздник под ключ  </div>
                    <ul>
                      <li>Праздник под ключ </li>
                    </ul>
                    </div>
                </div>
            </div>
          </div>


          <div class="with">
            <div class="content">
              <div class="title">С EasyFast</div>
               <div class="des">
                Вы не только экономите время. 
                Вы можете начать работать 
                и стать нашим проверенным исполнителем
                </div>
             <nuxt-link to="#"> <div class="btn"><span>СТАТЬ ИСПОЛНИТЕЛЕМ</span></div></nuxt-link>
            </div>
            <img src="../assets/imgs/ef.png" alt="">
          </div>

        <div class="snippet s-1">
          <img src="../assets/imgs/s-1.svg" alt="">

          <div class="content">
            <div class="m-title">Как это работает?</div>
            <div class="title">1.Этап </div>
            <div class="des">Зарегистрируйтесь на нашем сайте пройдя первоначальную проверку</div>
          </div>
        </div>

        <div class="snippet s-2">
          <img src="../assets/imgs/s-2.svg" alt="">

          <div class="content">
            <div class="title">2.Этап </div>
            <div class="des">дождитесь письма подтверждения
от нас </div>
          </div>
        </div>

  <div class="snippet s-3">
    
             <div class="btn show"><span>ПОСМОТРЕТЬ ЗАДАНИЯ</span></div>
          <img src="../assets/imgs/s-3.svg" alt="">

          <div class="content">
            <div class="title">3.Этап </div>
            <div class="des">Станьте нашим партнером и начинайте зарабатывать </div>
            <div class="btn"><span>ПОСМОТРЕТЬ ЗАДАНИЯ</span></div>
          </div>
        </div>



      <div class="advantages">
        <div class="title">Преимущества</div>
        <div class="advantages-cards">
          <div class="advantages-card">
            <img src="../assets/imgs/a-1.svg" alt="">
            <div class="text">Вы можете самостоятельно организовать Ваш праздник без лишних затрат</div>
          </div>
          <div class="advantages-card">
            <img src="../assets/imgs/a-2.svg" alt="">
            <div class="text">Вы можете самостоятельно организовать Ваш праздник без лишних затрат</div>
          </div>
          <div class="advantages-card">
            <img src="../assets/imgs/a-3.svg" alt="">
            <div class="text">Вы можете самостоятельно организовать Ваш праздник без лишних затрат</div>
          </div>
        </div>
      </div>


      <div class="reviews">
          <div class="title">Отзывы</div>

           <vCarousel :v-data="5" class="med" width="200px" height="200px"/>

      </div>


      <div class="news">
        <div class="title">Новости</div>

        
      <div class="cards">

        <div class="grid-1">
            <div @click="show=true" class="card-1">
              <div class="wrapper">
                <div class="title">
              Текст новости
                </div>
                <div class="des">
    Не следует, однако забывать, что постоянное информационно-пропагандистское обеспечение нашей деятельности в значительной степени обуславливает создание системы обучения кадров, соответствует насущным потребностям. Задача организации, 
    в особенности же начало повседневной ...
                </div>
                </div>
            </div>
             <div class="card-2">
            <img src="../assets/imgs/joke-1.png" alt="">
          </div>
          </div>
            <div class="grid-2">
              <div class="card-2">
            <img src="../assets/imgs/joke-1.png" alt="">
          </div>
          <div class="card-3">
            <img src="../assets/imgs/joke.png" alt="">
          </div>
          </div>
          </div>

        

      </div>
     </div>
      <transition name="slide-fade">
       <Modal :mt="500" @close="show=false" v-if="show">
            <img src="../assets/imgs/joke.png" width="100%" style="position:static;" alt="">
           <div class="title-modal">
              Текст новости
                </div>
                <div class="des-container">
                <div class="des-modal">
    Не следует, однако забывать, что постоянное информационно-пропагандистское обеспечение нашей деятельности в значительной степени обуславливает создание системы обучения кадров, соответствует насущным потребностям. Задача организации, 
    в особенности же начало повседневной ...
                </div>
                  <div class="des-modal">
    Не следует, однако забывать, что постоянное информационно-пропагандистское обеспечение нашей деятельности в значительной степени обуславливает создание системы обучения кадров, соответствует насущным потребностям. Задача организации, 
    в особенности же начало повседневной ...
                </div>
                </div>
       </Modal>
      </transition>

  </div>
</template>

<script>
import vCarousel from '../components/carousel/v-carousel.vue'
export default {
  data:()=>({
    show:false
  }),
  components:{
    vCarousel
  }
}
</script>


<style lang="scss" scoped>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css");
@import "../assets/styles/main.scss";
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active до версии 2.1.8 */ {
  transform: translateY(- 50vh);
  opacity: 0;
}

.show{
  display: none;
}
.center{
  @include center;
}
.title-modal{
  @include h1;
  margin: 30px 0;
}
.des-container{
  display: flex;
  flex-direction: column;
  gap:20px;
}





.news{
  margin: 150px 0 ;
  @include center{
    flex-direction: column;
  }
  .title{
    @include h1{
      margin: 0 0 40px 0;
    }
  }
  .cards{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 20px;
    .grid-1{
      cursor: pointer;
      display: grid;
      grid-template-columns: 1.5fr 1fr;
      grid-auto-rows: 1fr;
    }
    .grid-2{
      display: grid;
      grid-template-columns: 1fr 1.5fr;
      grid-auto-rows: 1fr;
      grid-gap: 30px;
      .card-1{
        width: 96%;
      }
    }
    .card-1{
      width: 436px;
      background: url("../assets/imgs/joke.png") no-repeat;
      backdrop-filter: blur(10px);
      background-size: cover;
      background-position: center ;
      .wrapper{
       width: 100%;
       height: 100%;
       padding: 48px 46px;
      background: rgba(255, 224, 128, 0.8);
      }
      .title{
        @include h2;
      }
    }

    @media (max-width:670px) {
      .grid-1,.grid-2{
        grid-template-columns: 1fr;
        display: flex;
        flex-direction: column;
        gap: 10px;
        width: 100%;
        div{
          width: 100%;
        }
        div img{
          width: 100%;
        }
        .wrapper{
          width: 100%;
        }
      }
      
    }
  }


}
.reviews{
  margin-top: 150px;
  @include center{
    flex-direction: column;
    gap: 40px;
  }
  .title{
    @include h1;
  }

}



.advantages{
  margin-top: 100px;
  @include center{
    flex-direction: column;
    gap: 40px;
  }
  .advantages-cards{
    @include center{
      gap:30px;
    }
  }
  .advantages-card{
    @include center{
      flex-direction: column;
      gap: 15px;
    }
  }
  .title{
    @include h1;
  }
  .text{
    @include h4{
      width: 50%;
      text-align: center;
    }
  }
  @media screen and (max-width:640px) {
    & .advantages-cards{
      flex-direction: column;
    }
  }
}





.snippet{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 230px;
  .content{
    display: flex;
    flex-direction: column;
    gap: 20px;
    width: 311px;
  }
  .m-title{
    @include h1;
  }
  .title{
    @include h2;
  }
  .des{
    @include h4;
  }
  @media screen and (max-width:1070px) {
    &{
      flex-direction: column-reverse;
      gap :0;
    }
    .content{
      width: 100%;
    }
    .btn{
      display: none;
    }
    .show{
      display: flex;
      margin: 20px 0;
    }
    .m-title{
      text-align: center;
    }
  }
  @media screen and (max-width:500px) {
    & > img{
      width: 90%;
    }
  }
}

.s-2{
  flex-direction: row-reverse;
  @media screen and (max-width:1070px) {
    flex-direction: column-reverse;
    gap:0;
  }
}

.s-3{
  margin-top: 60px;
}

.with{
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 50px;
  a{
    text-decoration: none;
  }
  .content{
    width: 45%;
    display: flex;
    flex-direction: column;
    gap: 30px;
    }
  .title{
    @include h1;
  }
  .des{
    @include h4;
  }
  .btn{
    background: linear-gradient(215.31deg, #F9F0C3 9.73%, #EFBB03 71.72%);
    border-radius: 100px;
    width: 246px;
    height: 43px;
    @include center;
    span{
      @include h3;
    }
  }

  @media (max-width:1070px) {
    &{
      flex-direction: column-reverse;
      margin: 30px 0 50px 0;
    }
    .content{
      width: 100%;
    }
  }
  @media (max-width:380px) {
    & > img{
      width: 95%;
    }
  }
}

.spezialition{
  padding: 90px 0;
  & > img{
    margin-left: 30%;
  }

  .container{
   
    width: 100%;
    display: flex;
    flex-direction: column;
    gap :30px;
    justify-content: center;
    align-items: center;

    &>.title{
      @include h1;
      margin: 71px 0;
    }

    .links{
        display: flex;
        justify-content: space-between;
        gap: 52px;
      .link{

        display: flex;
        flex-direction: column;
        gap:25px;

        &>.title{
          @include h3;
        }
      }
      ul li{
        list-style: none;
        @include h4;
        color: $tg;
      }
      ul{
        display: flex;
        flex-direction: column;
        gap: 15px;
      }
    }
  }


  @media (max-width:1125px) {
    &>img{
      margin-left: 0;
    }
  }
  @media (max-width:865px) {
    & > img{
      width: 95%;
    }
  }
  @media (max-width:555px) {
    .links{
      flex-wrap: wrap;
    }
  }
}


.about-part{
  width: 85%;
  margin-top: 200px;
  padding: 0 0 0 200px;
  display: flex;
  flex-direction: column;
  gap:30px;
  .title{
    @include h2;
  }
  .des{
    @include h3;
  }
  @media (max-width:750px) {
    &{
      width: 100%;
      padding: 0 30px;
    }
  }
}




  .welcome-part{
    position: relative;
    display: flex;
    justify-content: center;
    gap:100px;
    .main-img{
      z-index: 20;
    }
    .abs{
      position: absolute; 
      top: -80px;
      left: 0;
      z-index: 10;
    }
    .shadow{
      position: absolute;
      bottom: 0;
      left: 0;
    }

    .content{
      @include center{
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        gap:30px;


      }
      .title{
        @include h1;
      }
      .des{
        @include h2;
      }

      .btns{
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
        align-self: flex-end;
        justify-self: flex-end;
        flex-direction: column;
        gap :20px;
        .link a{
          color: $tg;
        }
        .btn{
        width: 196px;
        height: 42px;
        background: linear-gradient(215.31deg, #F9F0C3 9.73%, #EFBB03 71.72%);
        border-radius: 100px;
        @include center;
        span{
          @include h3{
            font-weight: 500;
          }
        }
        }
      }
    }

    @media  (max-width:1066px) {
      &{
        flex-direction: column;
        gap :0;
        align-items: center;
        justify-content: center;
      }
      .abs{
        left:30%;
      }
      &>img{
        width: 50%;
      }
      .content{
        background: $main-bg;
        border-radius: 50%;
        padding: 0 50px;
        text-align: center;
      }
    }

    @media (max-width:530px) {
      .content{
        padding: 0;
        border-radius: 0;
        background: transparent;
        &>img{
          margin: 50px 0 0 0;
        width: 100%;
        background: $main-bg;
        padding: 20px 30px;
      }
      .btns{
        align-items: center;
        justify-content: center;
        align-self: center;
        justify-self: center;
      }
      }
       
    }
    @media (max-width:1125px) {
     & .shadow{
        display: none;
      }
    }
  }


.main{
  width: 100%;
  background:
  url("../assets/imgs/bg1.png") no-repeat,
  url("../assets/imgs/bg2.png") no-repeat,
  url("../assets/imgs/bg.png") no-repeat,$main-bg;
 background-size: 100% auto;
 background-position: 0 -100px, 0 50px,0 1300px;
  display: flex;
  justify-content: center;
  

  .wrapper{
    width: 90%;
    padding: 30px 0;
  }


}
  @media screen and (max-width:1177px) {
   .main{
     background: #fff;
   } 
  }

  @media (max-width:630px) {
    .med{
      height: 300px;
    }
  }
</style>


