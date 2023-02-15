<script>

export default {
    name: 'ourBlog',
    data (){
        return{
            imgPosts: [
                {
                    img: '/src/assets/serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg',
                    date: 'May 24, 2018 by Alex',
                    title: 'Marketing ideas'
                },
                {
                    img: '/src/assets/Businessman-at-the-desk-in-his-office-resting--1024x768.jpg',
                    date: 'May 24, 2018 by Alex',
                    title: 'rest during working hours'
                },
                {
                    img: '/src/assets/simple-home-office-with-tree-PBXRXYB-large-1024x768.jpg',
                    date: 'May 24, 2018 by Alex',
                    title: 'develop your startup idea'
                },
            ]
        }
    }
}
</script>

<template>
    <section id="Blog">
        <!-- titel news and blog -->
        <h2 class="w-50 m-auto text-capitalize text-center">Latest news & our blog</h2>

        <div class="line-green justify-content-center mt-5">
            <div class="lineOne"></div>
            <div class="lineTwo"></div>
        </div>

        <!-- all posts -->
        <div class="posts my-5">
            <div class="container-fluid">
                <div class="row row-cols-3">
                    <div class="col" v-for="post in imgPosts">
                        <div class="post position-relative">
                            <img class="w-100 h-100 rounded" :src="post.img" alt="">
                            <div class="info-post m-auto rounded position-absolute bg-white p-4 text-capitalize">
                                <span>{{ post.date }}</span>
                                
                                <h5 class="align-middle mt-1">
                                    <font-awesome-icon class="circle align-middle" icon="fa-solid fa-circle" />
                                    {{ post.title }}
                                </h5>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- button -->
        <div class="d-flex justify-content-center">
            <button class="my-button mt-5">
                <a href="#">view all post</a>
            </button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.post{
    height: 350px;
    box-shadow: var(--shadow-black);

    .info-post{
        width: 90%;
        bottom: 0;
        left: 50%;
        transform: translate(-50%, 50%);
        box-shadow: var(--shadow-black);

        span{
            color: var(--text-gray-4);
            font-size: 0.8em;
        }

        .circle{
            font-size: 0.5em;
            color: var(--text-green);
        }
    }
}
</style>