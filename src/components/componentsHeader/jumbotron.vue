<script>
export default {
    name: 'Jumbotron',
    data (){
        return{
            currentSlide: 0,
            jumboImgs: [
                {
                    img: '/src/assets/Group-36-2x.png',
                    num: 1
                },
                {
                    img: '/src/assets/Group-35-2x.png',
                    num: 2
                },
                {
                    img: '/src/assets/Group-40-2x.png',
                    num: 3
                },
            ]
        }
    }
}
</script>

<template>
    <div class="jumbotron d-flex">
        <div class="title-jumbo ms-5 d-flex flex-column justify-content-center">
            <span>17 years of experience</span>
            <h1 class="text-capitalize">we are a <br> design agency</h1>
            <p>far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. 
                Separated they live in Bookmarkgrow right at the coast of the Semantics, a large language ocean.
                Separated they live in Bookmarkgrove.
            </p>

            <button class="my-button my-5">
                <a href="#">READ MORE</a>
            </button>

            <div class="socialsList d-flex justify-content-between align-items-center">
                <ul class="m-0 p-0">
                    <li class="text-uppercase d-inline-block">facebook</li>
                    <li class="text-uppercase d-inline-block">- instagram</li>
                    <li class="text-uppercase d-inline-block">- youtube</li>
                    <li class="text-uppercase d-inline-block">- twitter</li>
                </ul>

                <ul class="my-pagination p-1 border rounded-5">
                    <li class="d-inline-block" v-for="(slide, index) in jumboImgs">
                        <span @click="currentSlide = index" class="py-1 px-4 border rounded-5" :class="{'active' : currentSlide == index}">{{ slide.num }}</span>
                    </li>
                </ul>
            </div>
        </div>
    
        <div class="jumbo-img">
            <img :src="jumboImgs[currentSlide].img" alt="d">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.jumbotron{
    background-color: lightgray;
    overflow: hidden;

    .title-jumbo{

        span{
            font-size: 1.5em;
        }
        h1{
            font-size: 5em;
        }
        p{
            font-size: 1.5em;
        }
        .my-button{
            width: 150px;
        }
        .my-pagination{
            font-size: 1.5em;

            .active{
               background-color: green
            }
        }
    }
    .jumbo-img{
        width: 50%;

         > img{
            width: 1000px;
    }
    }
}
</style>