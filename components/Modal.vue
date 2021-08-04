<template>
<div class="container-main">
    <div class="main">
        <div class="container">
            <slot/>
        </div>
        <img @click="$emit('close')" src="../assets/imgs/close.svg" alt="">
    </div>
</div>
</template>

<style lang="scss" scoped>
.container-main{
    display: flex;
    align-items: center;
    justify-content: center;
    background: rgba($color: #3e97e4, $alpha: 0.8);
    
position: fixed;
top: 0;
left: 0;
z-index: 5001;
width: 100%;
height: 100vh;
overflow-x: scroll;
/* width */
&::-webkit-scrollbar {
   display: none;

}

/* Track */
&::-webkit-scrollbar-track {
  display: none;
}

/* Handle */
&::-webkit-scrollbar-thumb {
   display: none;

}

/* Handle on hover */
&::-webkit-scrollbar-thumb:hover {
   display: none;

}
}
.main{
    margin: 500px 0  100px 0;
    width: 60%;
    padding: 50px 80px;
    position: relative;
background: #F7F9FF;
box-shadow: -4px 4px 15px rgba(49, 69, 106, 0.2), 1px 1px 25px rgba(136, 165, 191, 0.15);
border-radius: 6px;
    img{
        position: absolute;
        top: 0;
        right: 0;
    }


   
}
 @media (max-width:533px) {
       .main{
            width: 90%;
            padding: 20px;
            margin: 300px 0 100px 0;
       } 
    }
</style>