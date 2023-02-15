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

                        <form action="#">
                            <div class="my-input-group d-flex align-items-center mt-5">
                                <input type="email" class="py-3 ps-4 w-100" placeholder="Enter Your Email Andress">
                                <input type="submit" value="SUBMIT" class="my-submit d-inline-block text-center pe-4 ms-3">
                            </div>
                        </form>
                    </div>
                </div>
                
                <div class="col">
                    <div class="p-5 work">
                        <p>what are you waiting for?</p>
                        <h2 class="mb-5 text-white">Let's Talk About Work</h2>

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
    background: var(--gradient-black);

    p{
    color: var(--text-gray-4);
    }

    .my-input-group{
    width: 70%;
    margin: auto;
    border-radius: 50px;
    background-color: var(--text-gray-2);

    input{
        border: none;
        border-radius: 50px;
        outline: none;
        background-color: transparent;
        color: white;
    }
    .my-submit{
        font-size: 0.8em;
    }

    }
}
.work{
    background: var(--gradient-green);

    p{
        color: var(--text-gray-3);
    }

    .my-button{
        box-shadow: 0px 0px 9px 0px rgba(0,0,0,0.5);
    }
}
</style>