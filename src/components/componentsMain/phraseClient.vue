<script>

export default {
    name: 'phraseClient',
}
</script>

<template>
    <section id="client">
        <div class="up-cover h-100 w-100 text-center d-flex justify-content-center align-items-center">
            <div class="text-client w-50 m-auto text-white">
                <p class="quote my-text-green"><font-awesome-icon icon="fa-solid fa-quote-left" /></p>
                <p class="phrase mt-4">
                    <em>
                        When it comes to barbequing, there are two main schools of thought for
                        the techniques thath you can use. Freshly scrambled eggs with applewood smoked bacon - are amazing!
                    </em>
                </p>

                <div class="client-img mt-5">
                    <img src="../../assets/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
                    <h3 class="mt-4 mb-0 my-text-green">LISSA DURBIN</h3>
                    <span>Client</span>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
#client{
    height: 800px;
    background-image: url(../../assets/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg);
    background-size: cover;
    background-position: center;

    .up-cover{
        background-color: rgba($color: #000000, $alpha: 0.7);

        .quote{
            font-size: 3em;
        }
        .phrase{
            font-size: 1.5em;
            color: var(--text-gray-3);
            line-height: 50px;
        }
        .client-img > img{
            width: 100px;
            clip-path: circle();
        }
    }
}
</style>