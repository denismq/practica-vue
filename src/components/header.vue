<template>
    <header class="main-header">
        <div class="main-header__logo"></div>
        <nav class="main-header__nav main-nav">
            <ul class="main-nav__items">
                <li class="main-nav__item"><a class="main-nav__link" href="#">Enlace 1</a></li>
                <li class="main-nav__item"><a class="main-nav__link" href="#">Enlace 2</a></li>
                <li class="main-nav__item"><a class="main-nav__link" href="#">Enlace 3</a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    
}
</script>
<style lang="scss" scoped>
//@import '~styles/main';
@import '~styles/style';

.main-header{
    font-family: $font-main;
    &__logo{
        width: 50px;
        height: 50px;
        background-color: gray;
    }
}
</style>



