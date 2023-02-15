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

                    <h2>
                        Our recent 
                        <span class="my-text-green">web designs</span>
                        & some examples of past
                        <span class="my-text-green">projects</span>
                    </h2>

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

        <div class="example-imgs">
            <div class="container-fluid position-relative">
                <div class="row row-cols-4 g-1">
                    <div class="col" v-for="singleImg in listProjects">
                        <div class="img-pro position-relative">
                            <img class="w-100 object-fit-cover" :src="singleImg.img" :alt="singleImg.img">
                        
                            <div class="up-img d-none position-absolute top-0 start-0 bottom-0 end-0">
            
                            </div>
                        </div>
                    </div>
                </div>

                <div class="badge position-absolute text-end bottom-50 end-0">
                    <div class="browse">
                        <a class="browse text-start p-2 my-1 rounded-start text-capitalize d-inline-block" href="#">
                            <font-awesome-icon class="me-1" icon="fa-solid fa-table-cells-large" />
                            browse demos
                        </a>
                    </div>
                    <div class="buy">
                        <a class="browse text-start p-2 my-1 rounded-start text-capitalize d-inline-block" href="#">
                            <font-awesome-icon class="me-1" icon="fa-solid fa-bag-shopping" />
                            buy now!
                        </a>
                    </div>
                    <div class="export">
                        <a class="browse text-start p-2 my-1 rounded-start text-capitalize d-inline-block" href="#">
                            <font-awesome-icon class="me-1" icon="fa-solid fa-file-export" />
                            export section
                        </a>
                    </div>
                </div>
            </div>
        </div>

        <div class="text-center mt-5">
            <button class="my-button mt-5">
                <a href="#">read more</a>
            </button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.example-imgs{
    overflow: hidden;
}
img{
    transition: all 0.2s;
}
.up-img{
    background: var(--gradient-green);
    opacity: 0.5;
}
.img-pro{
    transition: all 0.5s;

    &:hover{
    transform: scale(1.2);
    z-index: 30;
    .up-img{
        cursor: pointer;
        display: block !important;
    }
}
}
.badge{
    a{
        background-color: rgba($color: #000000, $alpha: 0.5);
        width: 120px;
        color: white;
    }
    a:hover{
        margin-right: 10px;
    }
}
.par{
    color: var(--text-gray-1);
}
</style>