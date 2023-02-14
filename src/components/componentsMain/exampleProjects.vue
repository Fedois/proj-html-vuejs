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
    <section id="projects">
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
            <div class="container-fluid text-center position-relative">
                <div class="row row-cols-4 g-1">
                    <div class="col" v-for="singleImg in listProjects">
                        <img class="w-100 object-fit-cover" :src="singleImg.img" alt="">
                    </div>
                </div>

                <div class="badge position-absolute bottom-50 end-0">
                    <div class="browse">
                        <a class="browse text-start p-2 my-1 rounded-start text-capitalize d-inline-block" href="#">
                            browse demos
                        </a>
                    </div>
                    <div class="buy">
                        <a class="browse text-start p-2 my-1 rounded-start text-capitalize d-inline-block" href="#">
                            buy now!
                        </a>
                    </div>
                    <div class="export">
                        <a class="browse text-start p-2 my-1 rounded-start text-capitalize d-inline-block" href="#">
                            export section
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.badge{
    a{
        background-color: rgba($color: #000000, $alpha: 0.5);
        width: 120px;
        color: white;
    }
}
</style>