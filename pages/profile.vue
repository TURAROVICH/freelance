<template>
    <div class="main">
        <div class="container">
             <div class="container-child">
                 <nuxt-child/>
             </div>
             <Profile/>
            
        </div>
    </div>
</template>

<script>
import Profile from '../components/profile/profile.vue'
export default {
    components:{
        Profile
    }
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/main.scss';
  .main{
      width: 100%;
      height: 100%;
      padding: 0 46px 120px 46px;
      background:$main-bg ;
      min-height: 100vh;
      margin-top: 10px;
      .container{
          width: 100%;
          height: 100%;
          display: grid;
          grid-template-columns: 2fr 1fr;
      }
      .container-child{
          width: 100%;
          padding: 30px;
          background: #fff;
            box-shadow: 1px 1px 25px rgba(136, 165, 191, 0.15);
            border-radius: 6px;
      }

      @media (max-width:1200px) {
        .container{
            grid-template-columns: 1fr ;
        }
    }
    @media (max-width:628px) {
        .main{
            padding: 0 0 120px 0;
        }
    }

    @media (max-width:380px) {
        .container-child{
            padding: 30px 0;
        }
    }
  }
</style>