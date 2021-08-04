<template>
     <div class="slide">
                  <div class="slide-head">
                    <div class="profile-data">
                      <img src="../../assets/imgs/review.svg" alt="">
                      <div class="review-data">
                        <div class="full-name">
                          Игорь Р.
                        </div>
                        <div class="data">
                          <span>Отзывы:</span>
                                <div>
                                <svg width="16" height="15" viewBox="0 0 16 15" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M3.23791 5.2168H1.23901C0.963039 5.2168 0.739273 5.43883 0.739273 5.71273V13.6475C0.739273 13.9213 0.963006 14.1434 1.23901 14.1434H3.23787C3.51384 14.1434 3.73761 13.9214 3.73761 13.6475V5.7127C3.73761 5.43883 3.51391 5.2168 3.23791 5.2168Z" fill="#667CA6"/>
                                <path d="M15.4772 6.53166C15.389 5.76234 14.6649 5.21707 13.8846 5.21707H9.98846C10.3196 4.62871 10.4973 2.96459 10.4894 2.2848C10.4763 1.15954 9.53731 0.257812 8.40335 0.257812H7.99098C7.71476 0.257812 7.49122 0.479616 7.49122 0.753752C7.49122 1.90055 7.04123 3.97049 6.19257 4.8127C5.62136 5.37955 5.13303 5.58495 4.49272 5.90251V13.3438C5.47306 13.6681 6.71777 14.1438 8.61496 14.1438H11.8841C12.9612 14.1438 13.8001 13.1538 13.3827 12.1078C14.0187 11.9359 14.4876 11.3571 14.4876 10.6723C14.4876 10.479 14.4501 10.294 14.3822 10.124C15.4539 9.83429 15.8483 8.52119 15.1045 7.69671C15.3778 7.39376 15.5285 6.97939 15.4772 6.53166Z" fill="#667CA6"/>
                                </svg>
                                <span>5</span>
                                </div>

                                <div>
                                  <svg width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M11.6155 9.15039L13.6145 9.15039C13.8905 9.15039 14.1143 8.92836 14.1143 8.65445L14.1143 0.71972C14.1143 0.445848 13.8905 0.223783 13.6145 0.223783L11.6155 0.223783C11.3395 0.223783 11.1157 0.445815 11.1157 0.71972L11.1157 8.65449C11.1157 8.92836 11.3395 9.15039 11.6155 9.15039Z" fill="#667CA6"/>
                                <path d="M0.374893 7.83553C0.455027 8.60485 1.11336 9.15012 1.82266 9.15012L5.36461 9.15012C5.0636 9.73848 4.90203 11.4026 4.9092 12.0824C4.92108 13.2076 5.77474 14.1094 6.8056 14.1094L7.18049 14.1094C7.43159 14.1094 7.63481 13.8876 7.63481 13.6134C7.63481 12.4666 8.04389 10.3967 8.81539 9.55449C9.33468 8.98764 9.7786 8.78224 10.3607 8.46468L10.3607 1.02334C9.46949 0.699087 8.33794 0.223442 6.61323 0.223442L3.64135 0.223442C2.66212 0.223442 1.89947 1.21344 2.27892 2.25943C1.70081 2.43134 1.27447 3.0101 1.27447 3.69492C1.27447 3.88818 1.30863 4.07316 1.3703 4.24316C0.396083 4.5329 0.0374899 5.846 0.713656 6.67049C0.465244 6.97343 0.328251 7.3878 0.374893 7.83553Z" fill="#667CA6"/>
                                </svg>
                                <span>1</span>
                                </div>
                                <div>
                                  <span>Рейтинг: </span> <i class="bi-star-fill" style="color:#EFBA03 "></i>
                                </div>


                        </div>
                      </div>
                    </div>
                    <div class="done">
                      <div class="title">Выполнено заданий:</div><span>5</span>
                    </div>
                  </div>
                  <div class="line">

                  </div>

                  <div class="slide-footer">
                    Не следует, однако забывать, что постоянное информационно-пропагандистское обеспечение нашей деятельности в значительной степени обуславливает создание системы обучения кадров, соответствует насущным потребностям. Задача организации, 
в особенности же начало повседневной работы по формированию позиции представляет собой интересный эксперимент проверки соответствующий условий активизации...
                  </div>

              </div>
</template>


<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/main.scss';

  .slide{
    min-width: 100%;
    padding: 0 20%;
    height: 100%;
    transition: all ease .9s;
    .slide-footer{
    width: 100%;
    @include h4;
    }


  .data {
    display: flex;
    gap: 10px;
    align-items: center;
   & > span{
    @include h4;
    color:$tg;

  }
  }
  .done{
    display: flex;
    .title{
      @include h4;
      color: $tg;

    }

    span{
      @include h4;
    }
  
  
  .line{
    height: 1px;
    width: 100%;
    background: #D6E4F0;
    margin: 10px 0;
  }


 

}
}
  .slide-head{
      width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;

  }
 .profile-data{
    display: flex;
   align-items: center;
   gap: 20px;
   .full-name{
     @include h3;
   }
  }

@media screen and (max-width:600px) {

     .slide-head{
         display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
    }
    .done{
      margin: 8px 0;
    }
  
}
 @media (max-width:874px) {
     .slide{
         padding: 0 ;
     }
 }
  @media (max-width:347px) {
     .profile-data{
         flex-direction: column;
     }
 }
</style>