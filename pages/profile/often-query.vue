<template>
    <div class="often-q">
        <div class="title">Частые вопросы</div>

        <div class="text">
            <div class="card">
                <div @click="show(1)" class="title"><span>Сколько предложений я получу?</span>  <div class="triangle-bottom" :class="{'active-arrow':content}"></div></div>
                <transition name="fade">  
               <div v-show="content" class="des ">
                   {{text}}
                   
               </div>
                </transition>  
            </div>

            <div class="card">
                <div @click="show(2)" class="title"><span>Обязательно ли выбирать исполнителя?</span>  <div class="triangle-bottom" :class="{'active-arrow':content2}"></div></div>
               <transition name="fade">  
               <div v-show="content2" class="des ">
                   {{text}}
                   
               </div>
                </transition>  
            </div>

            <div class="card">
                <div @click="show(3)" class="title"><span>Какую цену установить?</span>  <div class="triangle-bottom" :class="{'active-arrow':content3}"></div></div>
              <transition name="fade">  
               <div v-show="content3" class="des ">
                   {{text}}
                   
               </div>
                </transition>  
            </div>

            <div class="card">
                <div @click="show(4)" class="title"><span>Как оплачивать услуги? </span>  <div class="triangle-bottom" :class="{'active-arrow':content4}"></div></div>
                <transition name="fade">  
               <div v-show="content4" class="des ">
                   {{text}}
                   
               </div>
                </transition>  
            </div>

            <div class="card">
                <div @click="show(5)" class="title"><span>Как выбрать надежного исполнителя?</span>  <div class="triangle-bottom" :class="{'active-arrow':content5}"></div></div>
                <transition name="fade">  
               <div v-show="content5" class="des ">
                   {{text}}
                   
               </div>
                </transition>  

            </div>

            
            <div class="card">
                <div @click="show(6)" class="title"><span>Как не выбрать исполнителем мошенника?</span>  <div class="triangle-bottom " :class="{'active-arrow':content6}"></div></div>
                <transition name="fade">  
             <div v-show="content6" class="des ">
                   {{text}}
               </div>
                </transition>
            </div>

            
        </div>
    </div>
</template>

<script>
export default {
    data:()=>({
        text:`Не следует, однако забывать, что постоянное информационно-пропагандистское обеспечение нашей деятельности в значительной степени обуславливает создание системы обучения кадров, соответствует насущным потребностям. Задача организации, 
в особенности же начало повседневной работы по формированию позиции представляет собой интересный эксперимент проверки соответствующий условий активизации...
          `,
          content:false,
          content2:false,
          content3:false,
          content4:false,
          content5:false,
          content6:false,
    }),
    methods:{
        show(id){
            if(id == 1 ){
                    this.content=!this.content
                    this.content2=false
                    this.content3=false
                    this.content4=false
                    this.content5=false
                    this.content6=false
            } 
            if(id == 2 && !this.conten2){
                  this.content2=!this.content2
                    this.content=false
                    this.content3=false
                    this.content4=false
                    this.content5=false
                    this.content6=false
            } 
            if(id == 3 && !this.conten3){
                  this.content3=!this.content3
                    this.content=false
                    this.content2=false
                    this.content4=false
                    this.content5=false
                    this.content6=false
            } 
            if(id == 4 && !this.conten4){
                  this.content4=!this.content4
                    this.content=false
                    this.content2=false
                    this.content3=false
                    this.content5=false
                    this.content6=false
            } 
            if(id == 5 && !this.conten5){
                  this.content5=!this.content5
                    this.content=false
                    this.content2=false
                    this.content3=false
                    this.content4=false
                    this.content6=false
            } 
             if(id == 6 && !this.conten6){
                   this.content6=!this.content6
                    this.content=false
                    this.content2=false
                    this.content3=false
                    this.content4=false
                    this.content5=false
            } 
        }
    }

}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active до версии 2.1.8 */ {
  opacity: 0;
}
.often-q{
    width: 100%;
    &>.title{
        @include h2;
    }
    .text{
        margin-top: 37px;
        width: 100%;
    }
    .card{
        display: flex;
        flex-direction: column;
        gap:30px;
        margin: 20px 0 0 0;
        .title{
            display: flex;
            gap: 4px;
            align-items: center;
            @include h3{
                color:#4097E3;
            }
        }
        .des{
            @include h4;
            margin-bottom: 50px;
        }
    }
 .triangle-bottom {
    width: 0;
    height: 0;
    border-left: 7px solid transparent;
    border-right: 7px solid transparent;
    border-top: 8px solid #4097E3;;
}
.active-arrow{
    transition: all .5s ease;
    transform: rotate(180deg);
}

@media (max-width:452px) {
    .card .title{
       width: 250px;
       justify-content: space-between;
    }
    .card{
        width: 90%;
        margin: 20px auto;
    }
}
@media (max-width:288px) {
    .card .title{
        width: 220px;
    }
}
}
</style>