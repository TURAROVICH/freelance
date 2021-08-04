<template>
    <div @click="res=!res" class="switch" :class="{'active':res}">
        <div :class="{'right':res ,'switch-btn':!res}"></div>
    </div>
</template>

<script>
export default {
    data:()=>({
        res:false
    }),
    watch:{
        res(){
            return this.$emit('res',this.res)
        }
    }
}
</script>

<style lang="scss" scoped>
.switch{
    position: relative;
    width: 36px;
    height: 17px;
    border-radius: 16px;
    padding: 5px;
    background: #E4E7F5;
/* 3 */

    box-shadow: inset -3px -3px 7px #FFFFFF, inset 1px 1px 3px rgba(136, 165, 191, 0.48);
    .switch-btn{
        height: 15px;
        width: 15px;
        border-radius: 50%;
        background: #fff;
        position: absolute;
        top:1px;
        left:0;
        transition: all .5s ease;

    }
    .right{
    right: 0;
     height: 15px;
        width: 15px;
        border-radius: 50%;
        background: #fff;
        position: absolute;
        top: 1px;
        transition: all .5s ease;
    }
}
.active{
    background: linear-gradient(215.31deg, #64DBF5 9.73%, #2567E7 71.72%);
    box-shadow: inset 3px 3px 7px #2E127C, inset 1px 1px 3px rgba(136, 165, 191, 0.48);
}

</style>