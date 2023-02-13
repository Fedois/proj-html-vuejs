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
        linkNav: Array
    }
}
</script>

<template>
    <header>
        <div class="top-header text-white py-2 px-5 d-flex justify-content-between align-items-center">
            <div class="number">
                <p class="m-0 me-4 d-inline-block">{{ numOne }}</p>
                <p class="m-0 me-4 d-inline-block"> {{ numTwo }}</p> 
            </div>

            <div class="icons">
                <ul class="m-0">
                    <li class="d-inline-block">
                        <a class="text-white" href="#">
                            <font-awesome-icon class="mx-2" icon="fa-brands fa-facebook-f" />
                        </a>
                    </li>
                    <li class="d-inline-block">
                        <a class="text-white" href="#">
                            <font-awesome-icon class="mx-2" icon="fa-brands fa-twitter" />
                        </a>
                    </li>
                    <li class="d-inline-block">
                        <a class="text-white" href="#">
                            <font-awesome-icon class="mx-2" icon="fa-brands fa-pinterest-p" />
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <div class="header-bottom row row-cols-3 p-4">
            <div class="logo">
                <img src="../../assets/cropped-Group-39-2x.png" alt="Phlox | Business">
            </div>

            <nav class="text-center">
                <ul class="m-0 d-flex align-items-center h-100">
                    <li class="mx-3 text-uppercase" v-for="link in linkNav">
                        <a href="#" class="text-decoration-none text-dark">{{ link }}</a>
                    </li>
                </ul>
            </nav>

            <div class="purchase text-end">
                <button class="my-button">purchase</button>
                <font-awesome-icon class="ms-3" icon="fa-solid fa-magnifying-glass" />
            </div>
        </div>

        <jumbotron />
        
    </header>
</template>

<style lang="scss" scoped>
.top-header{
    background-color: black;
}
nav > ul{
    list-style: none;
}
</style>