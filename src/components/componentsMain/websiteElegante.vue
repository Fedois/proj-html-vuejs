<script>
export default {
    name: 'websiteElegant',
    data (){
        return{
            listImprove: [
                {
                    img: '/src/assets/speed-optimization.png',
                    title: 'Speed Optimization',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
                {
                    img: '/src/assets/cloud.png',
                    title: 'Cloud Solutions',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
                {
                    img: '/src/assets/ipad-logo.png',
                    title: 'Website Design',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
                {
                    img: '/src/assets/cronometro-icon.png',
                    title: 'Online Marketing',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
            ]
        }
    }
}
</script>

<template>
    <section id="website" class="d-flex justify-content-between">
        <div class="makeSite ps-3 pe-5">
            <h2 class="text-capitalize">We are here to make your website look more elegant and stylish!</h2>

            <div class="line-green">
                <div class="lineOne"></div>
                <div class="lineTwo"></div>
            </div>

            <button class="my-button mt-4">
                <a href="#">view all</a>
            </button>
        </div>
        
        <div class="cards-site">
            <div class="container">
                <div class="row g-3">
                    <div class="col-6" v-for="card in listImprove">
                        <div class="p-4 border">
                            <div class="img-icon mb-4">
                                <img :src="card.img" :alt="card.title">
                            </div>

                            <div class="info-card">
                                <h4>{{ card.title }}</h4>
                                <p class="mb-0">{{ card.info }}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.makeSite{
    width: 40%;
}
.cards-site{
    width: 60%;

    .img-icon{
        height: 50px;
        > img{
            width: 50px;
        }
    }
}
</style>