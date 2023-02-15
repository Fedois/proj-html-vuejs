<script>
export default {
    name: 'AppFooter',
    props: {
        logo: Object,
        quickLinks: Array,
        contacts: Array,
        map: String,
        icons: Array
    }
}
</script>

<template>
    <footer>
        <div class="list-foot container-fluid mb-5">
            <div class="row row-cols-4">
                <div class="col logo-foot">
                <div class="p-3">
                    <img :src="logo.img" :alt="logo.nameLogo">
                    <p class="mt-4">
                        While the lovely valley teems vith vapour around me, and the meridian sun strikes the upper surface of the impenetrble foliage of my trees.
                        While the lovely valley teems with vapour arond me.
                    </p>
                </div>
                </div>
                <div class="col links-foot">
                <div class="p-3">
                    <h4>quick links</h4>

                    <div class="line-green">
                        <div class="lineOne"></div>
                        <div class="lineTwo"></div>
                    </div>

                    <ul class="links p-0">
                        <li class="m-0 text-uppercase py-1" v-for="link in quickLinks">
                            <a href="#">{{ link }}</a>
                        </li>
                    </ul>
                </div>
                </div>
                
                <div class="col contacts-foot">
                <div class="p-3">
                    <h4>contacts</h4>

                    <div class="line-green">
                        <div class="lineOne"></div>
                        <div class="lineTwo"></div>
                    </div>

                    <ul class="p-0">
                        <li v-for="info in contacts">
                            <p class="py-2">{{ info.street }}</p>
                            <p class="py-2">{{ info.email }}</p>
                            <p class="py-2">{{ info.number }}</p>
                        </li>
                    </ul>

                </div>
                </div>
                <div class="col map-foot">
                <div class="p-3">
                    <h4>location on map</h4>

                    <div class="line-green">
                        <div class="lineOne"></div>
                        <div class="lineTwo"></div>
                    </div>

                    <div class="map-img">
                        <img class="w-100 h-100" :src="map" alt="">
                    </div>
                </div>
                </div>
            </div>
        </div>

        <div class="bottom-foot p-4 d-flex justify-content-between align-items-center text-white">
            <p class="text-uppercase m-0">2020 phlox business theme.</p>

            <div class="icons-social">
                <a href="#" v-for="singleIcon in icons">
                    <font-awesome-icon class="mx-2 text-white" :icon="singleIcon.icon" />
                </a>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.list-foot *{
    color: var(--text-gray-1);
}
h4{
    text-transform: uppercase;
}
ul{
    list-style: none;

    a:hover{
        border-bottom: 3px solid var(--text-green);
        color: var(--text-gray-1);
    }
}
.map-img{
    height: 200px;

    img{
        object-fit: contain;
    }
}
.bottom-foot{
    background: rgb(0,12,11);
    background: linear-gradient(270deg, rgba(0,12,11,1) 32%, rgba(51,51,51,1) 89%);

    > *{
        font-size: 0.8em;
        color: var(--text-gray-4);
    }
}
</style>