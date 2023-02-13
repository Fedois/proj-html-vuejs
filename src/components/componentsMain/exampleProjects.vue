<script>
export default {
    name: 'exampleProjects',
    data() {
        return{
            listProjects: [
                {
                    img: '/src/assets/ina-soulis-227104-unsplash-1024x1024.jpg'
                },
                {
                    img: '/src/assets/sunisa-misa-531163-unsplash-1024x1024.jpg'
                },
                {
                    img: '/src/assets/355H-1024x1024.jpg'
                },
                {
                    img: '/src/assets/photo-1448932252197-d19750584e56-1024x1024.jpg'
                },
                {
                    img: '/src/assets/business-competition-PB366D8-1024x1024.jpg'
                },
                {
                    img: '/src/assets/cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg'
                },
                {
                    img: '/src/assets/aa9a4539-PQGJ7HU-1024x1024.jpg'
                },
                {
                    img: '/src/assets/cody-davis-253928-unsplash-1024x1024.jpg'
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="text-project">
            <div class="container-fluid d-flex mb-5">
                <div class="title w-50">
                    <div class="line-green">
                        <div class="lineOne"></div>
                        <div class="lineTwo"></div>
                    </div>

                    <h2>Our recent web designs & some examples of past projects</h2>

                    <div class="line-green">
                        <div class="lineOne"></div>
                        <div class="lineTwo"></div>
                    </div>
                </div>
                
                <div class="par w-50 align-self-end">
                    <p>
                        far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. 
                        Separated they live in Bookmarkgrow right at the coast of the Semantics, a large language ocean.
                        Separated they live in Bookmarkgrove.
                    </p>
                </div>
            </div>
        </div>

        <div class="example-img">
            <div class="container-fluid text-center">
                <div class="row row-cols-4 g-1">
                    <div class="col" v-for="img in listProjects">
                        <img class="w-100 object-fit-cover" :src="img.img" alt="">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>

</style>