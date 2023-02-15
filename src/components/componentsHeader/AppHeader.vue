<script>
import Jumbotron from './jumbotron.vue'
export default {
    name: 'AppHeader',
    components: {
        Jumbotron
    },
    props: {
        numOne: String,
        numTwo: String,
        logo: Object,
        linkNav: Array,
        icons: Array
    }
}
</script>

<template>
    <header>
        <!-- inizio top header -->
        <div class="top-header text-white py-2 px-5 d-flex justify-content-between align-items-center">
            <div class="number">
                <p class="m-0 me-4 d-inline-block">{{ numOne }}</p>
                <p class="m-0 me-4 d-inline-block"> {{ numTwo }}</p> 
            </div>

            <div class="icons">
                <ul class="m-0">
                    <li class="d-inline-block">
                        <a class="text-white" href="#" v-for="singleIcon in icons">
                            <font-awesome-icon class="mx-2" :icon="singleIcon.icon" />
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <!-- inizio header navigation -->
        <div class="header-bottom bg-white d-flex justify-content-between p-4">
            <div class="logo">
                <img :src="logo.img" :alt="logo.nameLogo">
            </div>

            <nav class="text-center">
                <ul class="m-0 d-flex align-items-center h-100">
                    <li class="mx-3" v-for="link in linkNav">
                        <a href="#" class="text-decoration-none text-uppercase">{{ link }}</a>
                    </li>
                </ul>
            </nav>

            <div class="purchase text-end">
                <button class="my-button">
                    <a href="#">purchase</a>
                </button>
                <font-awesome-icon class="mx-3" icon="fa-solid fa-magnifying-glass" />
            </div>
        </div>

        <jumbotron />
        
    </header>
</template>

<style lang="scss" scoped>
header > div:not(#jumbotron){
  position: sticky;
  top: 0;
}
.top-header{
    background-color: var(--bg-gray-2);
}
nav > ul{
    list-style: none;

    a{
        color: var(--text-gray-1);
    }

    a:hover{
        border-bottom: 3px solid;
        border-color: var(--text-green);
    }
}
</style>