<template>
    <div class="main-cnt">
        <div class="about-text">
            <div class="title">Стоимость одной  категории 100 ₽ </div>

            <div class="right-text">
                <div>* Первый месяц подписка на выбранные категории бесплатна.</div>
                <div>
                Далее подписка на выбранные категории действительна в течение месяца.</div>
            </div>
        </div>

        <div class="sub-container">
            <div class="title">Выбирите категорию</div>

            <div class="justify">
                <div class="card">
                    <img src="../../assets/imgs/ball.svg" alt="">

                    <div class="title">Декор, инвентарь </div>
                    <div class="swic">
                       <switch-1 />
                       <span>Шарики </span>
                    </div>
                      <div class="swic">
                       <switch-1 start />
                       <span>Флористика  </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Декор  </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Транспорт </span>
                    </div>
                </div>
                <div class="card">
                    <img src="../../assets/imgs/person.svg" alt="">

                    <div class="title">Персонал </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Ведущие </span>
                    </div>
                      <div class="swic">
                       <switch-1 start />
                       <span>Аниматоры    </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Фото/видеосъемка   </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Артисты </span>
                    </div>
                  <div class="swic">
                       <switch-1 start />
                       <span>Стилисты </span>
                    </div>
                </div>
            </div>
            <div class="justify">
                <div class="card">
                    <img src="../../assets/imgs/geo.svg" alt="">

                    <div class="title">Площадки  </div>
                    <div class="swic">
                       <switch-1 />
                       <span>Рестораны  </span>
                    </div>
                      <div class="swic">
                       <switch-1 start />
                       <span>Кафе  </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Банкетные залы   </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Кейтеринг </span>
                    </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Детские площадки </span>
                    </div>
                </div>
                <div class="card">
                    <img src="../../assets/imgs/key.svg" alt="">

                    <div class="title">Праздник под ключ  </div>
                    <div class="swic">
                       <switch-1 start />
                       <span>Праздник под ключ </span>
                    </div>
                    
                </div>
            </div>
            <div class="btn-container">
                <div class="title">К оплате: 300 ₽</div>
                <div class="btn-blue"><span>ОПЛАТИТЬ</span></div>
            </div>
        </div>
        
    </div>
</template>

<script>
import Switch1 from '../../components/switch.vue'
export default {
    components:{Switch1}
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
.swic {
display: flex;
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

.main-cnt{
    width: 100%;
    padding: 30px;

    .sub-container{
        width: 70%;
        margin: 30px auto;
        .justify{
            width: 100%;
            display: flex;
            justify-content: space-between;
            margin: 55px 0 0 0;
            
            .card{
                display: flex;
                flex-direction: column;
                gap :18px;
                img{
                    margin: 0 0 30px 0;
                    height: 77px;
                    width: 80px;
                }
            }
            .title{
                @include h3;
            }
        }
        &>.title{
            @include h2{
                text-align: center;
            }
        }
    }


    .about-text{
        width: 100%;
        display: flex;
        justify-content: space-between;
        .title{
            @include h3;
        }
        .right-text{
            width: 40%;
            display: flex;
            flex-direction: column;
            gap :15px;
            div{
                @include h5;
                color:$tg;
            }
        }
    }
    .btn-container{
        width: 80%;
        margin: 70px auto 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-between;
        .title{
            @include h2;
        }
        .btn-blue{
            @include btn-blue{
                width: 173px;
            }
        }
    }
    @media (max-width:870px) {
        .sub-container{
            width: 90%;
        }
    }
     @media (max-width:721px) {
        .btn-container{
            width: 95%;
        }
    }
    @media (max-width:621px) {
        .about-text{
            flex-direction: column;
            .right-text{
                margin: 20px 0 0 0;
            }
        }
    }
      @media (max-width:525px) {
        .btn-container{
            flex-direction: column;
            justify-content: center;
            gap: 20px;
        }
        .justify{
            flex-direction: column;
            gap :70px;
        }
    }
}
</style>
