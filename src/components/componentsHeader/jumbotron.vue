<script>
export default {
    name: 'Jumbotron'
}
</script>

<template>
    <div class="jumbotron position-relative">
        <div class="title position-absolute">
            <span>17 years of experience</span>
            <h1 class="text-capitalize">we are a <br> design agency</h1>
            <p>far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. 
                Separated they live in Bookmarkgrow right at the coast of the Semantics, a large language ocean.
                Separated they live in Bookmarkgrove.
            </p>

            <button class="my-button my-5">
                <a href="#" class="text-dark">READ MORE</a>
            </button>

            <div class="socialsList d-flex justify-content-between align-items-center">
                <ul class="m-0 p-0">
                    <li class="text-uppercase d-inline-block">facebook</li>
                    <li class="text-uppercase d-inline-block">- instagram</li>
                    <li class="text-uppercase d-inline-block">- youtube</li>
                    <li class="text-uppercase d-inline-block">- twitter</li>
                </ul>

                <ul class="my-pagination m-0 p-1 border rounded-5">
                    <li class="py-1 px-4 d-inline-block border rounded-5"><a href="#">1</a></li>
                    <li class="py-1 px-4 d-inline-block border rounded-5"><a href="#">2</a></li>
                    <li class="py-1 px-4 d-inline-block border rounded-5"><a href="#">3</a></li>
                </ul>
            </div>
        </div>
    
        <div class="jumbo-img">
            <img class="position-absolute" src="../../assets/Group-36-2x.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.jumbotron{
    background-color: lightgray;
    overflow: hidden;
    height: 1000px;

    .title{
        width: 40%;
        margin: 150px;

        span{
            font-size: 1.5em;
        }
        h1{
            font-size: 5em;
        }
        p{
            font-size: 2em;
        }
        .my-pagination{
            font-size: 1.5em;
        }
    }
    .jumbo-img{
        width: 60%;

         > img{
        width: 70%;
        top: -5%;    
        right: -10%;
    }
    }
}
</style>