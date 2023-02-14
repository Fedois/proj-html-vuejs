<script>

export default {
    name: 'startProject',
    data (){
        return {
            listSponsor: [
                {
                    img: '/src/assets/client-1-2x.png',
                    name: 'client-1'
                },
                {
                    img: '/src/assets/client-9-2x.png',
                    name: 'client-1'
                },
                {
                    img: '/src/assets/client-7-2x.png',
                    name: 'client-1'
                },
                {
                    img: '/src/assets/client-3-2x.png',
                    name: 'client-1'
                },
                {
                    img: '/src/assets/client-4-2x.png',
                    name: 'client-1'
                },
                {
                    img: '/src/assets/client-5-2x.png',
                    name: 'client-1'
                },
            ]
        }
    }
}
</script>

<template>
    <section id="new-project">
        <div class="container-fluid text-center">
            <div class="row row-cols-2">
                <div class="col">
                    <div class="p-5 new-pro text-white">
                        <p>Are you ready?</p>
                        <h2>Start a New Project</h2>

                        <form action="">
                            <div class="my-input-group d-flex align-items-center mt-5">
                                <input type="email" class="p-2 ps-4 w-100" placeholder="Enter Your Email Andress">
                                <span class="d-inline-block text-dark text-center pe-4 ms-3">SUBMIT</span>
                            </div>
                        </form>
                    </div>
                </div>
                
                <div class="col">
                    <div class="p-5 work">
                        <p>what are you waiting for?</p>
                        <h2 class="mb-5">Let's Talk About Work</h2>

                        <button class="my-button">
                            <a href="#">start now</a>
                        </button>
                    </div>
                </div>
            </div>
        </div>

        <div class="container-fluid mt-5 sponsor-imgs text-center">
            <div class="row row-cols-6 align-items-center">
                <div class="col mt-5" v-for="singleImg in listSponsor">
                    <div class="p-3">
                        <img :src="singleImg.img" alt="">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.new-pro, .work{
    height: 300px;
}
.new-pro{
    background: rgb(0,12,11);
    background: linear-gradient(270deg, rgba(0,12,11,1) 32%, rgba(51,51,51,1) 89%);

    .my-input-group{
    width: 70%;
    margin: auto;
    border-radius: 50px;
    background-color: white;

    input{
        border: none;
        border-radius: 50px;
        outline: none;
    }
    span{
        font-size: 0.8em;
        background-color: white;
        border-radius: 0 50px 50px 0;
    }

    }
}
.work{
    background-color: green;
}
</style>