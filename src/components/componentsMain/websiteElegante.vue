<script>
export default {
    name: 'websiteElegant',
    data (){
        return{
            listImprove: [
                {
                    icon: 'fa-solid fa-gauge-high',
                    title: 'Speed Optimization',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
                {
                    icon: 'fa-solid fa-cloud',
                    title: 'Cloud Solutions',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
                {
                    icon: 'fa-solid fa-tablet-screen-button',
                    title: 'Website Design',
                    info: 'Far far away, behind the word mountains, far from the countries Vokaia Separated...'
                },
                {
                    icon: 'fa-solid fa-stopwatch',
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
            <h2 class="text-capitalize">We are here to make your 
                <span class="my-text-green">website</span> 
                look more
                <span class="my-text-green">elegant</span> 
                and stylish!
            </h2>

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
                <div class="row g-4">
                    <div class="col-6" v-for="card in listImprove">
                        <div class="my-box p-4 mb-2 rounded-3">
                            <div class="icon mb-4">
                                <font-awesome-icon :icon="card.icon" />
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

    p{
        color: var(--text-gray-1);
    }
    .my-box{
        box-shadow: var(--shadow-black);
        transition: all 0.3s;
    }

    .my-box:hover{
        cursor: pointer;
        background: var(--gradient-green);
        transform: scale(1.01);
        box-shadow: var(--shadow-green);
    }

    .icon{
        font-size: 3em;
    }
}
</style>