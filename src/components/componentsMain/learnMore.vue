<script>
export default {
    name: 'learnMore',
}
</script>

<template>
    <section class="learnMore d-flex alig-items-center">
        <div class="learn-sx w-50">
            <div class="learn-img position-relative">
                <img class="back-img w-100" src="../../assets/busy-architect-PYVKWM4-1024x872.jpg" alt="busy-architect">
                <div class="bg-up position-absolute top-0 start-0 end-0 bottom-0"></div>
                <img class="img-busWoman w-100 position-absolute" src="../../assets/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
            </div>
        </div>

        <div class="learn-dx w-50">
            <div class="text-learn">
                <h2 class="h-100 align-middle">Learn more about our missions</h2>

                <div class="line-green">
                    <div class="lineOne"></div>
                    <div class="lineTwo"></div>
                </div>

                <p>far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. 
                    Separated they live in Bookmarkgrow right at the coast of the Semantics, a large language ocean.
                    Separated they live in Bookmarkgrove.
                </p>

                <button class="my-button mt-3">
                    <a href="#">learn more</a>
                </button>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.learn-sx{
    img{
    object-fit: cover;
    }
    .learn-img{
        width: 500px;
        height: 500px;
    }
    .bg-up{
        background-color: rgba($color: green, $alpha: 0.8);
    }
    .img-busWoman{
        top: 15%;
        left: 15%;
        width: 500px;
        height: 500px;
    }
}
.learn-dx{
    margin: auto 0;

    .text-learn{
        width: 500px;
    }
}
</style>