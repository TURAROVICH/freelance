<template>
<div class="container">
<div class="wrapper">
     <div class="slider-container" :style="{'margin-left':`-${currenSlide}00%`}">
            <v-item
            v-for="i of vData" :key="i"
            /> 


    </div>
</div>
<div class="nav">
<svg  v-for="i of vData-1" :key="i" @click="slide(i)" width="12" height="12" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg">
            <ellipse cx="3.5" cy="3.49105" rx="3.5" ry="3.49105" :fill="fill"/>
</svg>
</div>
</div>
</template>

<script>
import vItem from './v-carousel-item.vue'
export default {
    props:['v-data'],
    data:()=>({
        currenSlide:0,
        fill:'#9AB3D9',
    }),
    methods:{
        slide(id){
            if(id!=this['v-data']){
            let count = (id*2)
            this.currenSlide = count
            }
        }
    },
    components:{
       vItem
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
.container{
    width: 90%;
    @include center{
        flex-direction: column;
    }
}
.nav{
    @include center{
        gap: 5px;
    }
}
.slider-container{
       transition: all ease .9s;
  width: 100%;
  min-height: 185px;
  display: flex;
  }


.wrapper{
    position: relative;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
}

 


@media screen and (max-width:600px) {
   .slider-container{
    width: 100%;
  }
  .nav{
      margin-top: 50px;
  }
}
 
</style>