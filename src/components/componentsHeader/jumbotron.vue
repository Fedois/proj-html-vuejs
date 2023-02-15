<script>
export default {
    name: 'Jumbotron',
    data (){
        return{
            currentSlide: 0,
            listSocial: ['facebook', 'instagram', 'youtube', 'twitter'],
            jumboImgs: [
                {
                    img: '/src/assets/Group-36-2x.png',
                    num: '01'
                },
                {
                    img: '/src/assets/Group-35-2x.png',
                    num: '02'
                },
                {
                    img: '/src/assets/Group-40-2x.png',
                    num: '03'
                },
            ]
        }
    }
}
</script>

<template>
    <div id="jumbotron" class="d-flex">
        <div class="title-jumbo ms-5 d-flex flex-column justify-content-center">
            <span class="my-text-green text-uppercase">17 years of experience</span>
            
            <h1 class="text-capitalize">we are a <br> designe <span class="my-text-green">agency</span> </h1>

            <div class="line-green">
                <div class="lineOne"></div>
                <div class="lineTwo"></div>
            </div>
            
            <p>
                far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. 
                Separated they live in Bookmarkgrow right at the coast of the Semantics, a large language ocean.
                Separated they live in Bookmarkgrove.
            </p>

            <button class="my-button my-5">
                <a href="#">READ MORE</a>
            </button>

            <div class="socialsList d-flex justify-content-between align-items-center">
                <ul class="m-0 p-0">
                    <li class="text-uppercase d-inline-block me-2" v-for="social in listSocial">
                       <strong>
                            - <a href="#"> {{ social }}</a>
                       </strong> 
                    </li>
                </ul>

                <ul class="my-pagination p-1 rounded-5">
                    <li class="d-inline-block" v-for="(slide, index) in jumboImgs">
                        <span @click="currentSlide = index" class="py-1 px-3 rounded-5" :class="{'active' : currentSlide == index}">{{ slide.num }}</span>
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
#jumbotron{
    background-color: var(--bg-gray-1);
    overflow: hidden;

    .title-jumbo{

        > span, p{
            font-size: 1em;
        }
        > span{
            letter-spacing: 10px;
        }
        > h1{
            font-size: 5em;
        }
        > p{
            color: var(--text-gray-1);
        }
        strong > a{
            color: black;
        }
        .my-button{
            width: 170px;
        }
        .my-pagination{
            font-size: 1.5em;
            background: var(--gradient-black);
            color: var(--text-gray-3);
            box-shadow: 0px 0px 9px 0px rgba(0,0,0,0.78);


            &:hover{
                cursor: pointer;
            }

            .active{
                background: var(--gradient-green);
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