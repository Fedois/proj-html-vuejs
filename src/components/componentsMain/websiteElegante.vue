<script>
export default {
    name: 'websiteElegant'
}
</script>

<template>
    <section class="website d-flex justify-content-between">
        <div class="makeSite ps-3 pe-5">
            <h2 class="text-capitalize">We are here to make your website look more elegant and stylish!</h2>

            <div class="line-green d-flex my-4">
                <div class="lineOne rounded me-2"></div>
                <div class="lineTwo rounded"></div>
            </div>

            <button class="my-button mt-4">VIEW ALL</button>
        </div>
        
        <div class="cards-site">
            <div class="container">
                <div class="row g-3">
                    <div class="col-6">
                        <div class="p-3 border">
                            <h4>Speed optimization</h4>
                            <p>Far far away, behind the word mountains, far from the countries Vokaia Separated...</p>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="p-3 border">
                            <h4>Speed optimization</h4>
                            <p>Far far away, behind the word mountains, far from the countries Vokaia Separated...</p>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="p-3 border">
                            <h4>Speed optimization</h4>
                            <p>Far far away, behind the word mountains, far from the countries Vokaia Separated...</p>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="p-3 border">
                            <h4>Speed optimization</h4>
                            <p>Far far away, behind the word mountains, far from the countries Vokaia Separated...</p>
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

    h2{
        font-size: 2.5em;
    }
}
.cards-site{
    width: 60%;
}
.lineOne{
    background-color: red;
    height: 5px;
    width: 15px;
}
.lineTwo{
    background-color: green;
    height: 5px;
    width: 40px;
}
</style>