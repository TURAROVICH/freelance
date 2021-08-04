<template>
    <div class="container-modal" style="gap:30px;">
                    <div class="title">
                        Вход
                    </div>
                    <input type="email" placeholder="E-mail">
                    <div @click="$emit('send')" class="btn">
                        <span>ОТПРАВИТЬ</span>
                    </div>
                </div>
</template>


<style lang="scss" scoped>
@import '../../assets/styles/main.scss';
@import '../../assets/styles/auth.scss';
</style>