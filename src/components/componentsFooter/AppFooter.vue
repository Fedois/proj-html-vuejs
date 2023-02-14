<script>
export default {
    name: 'AppFooter',
    props: {
        logo: Object,
        quickLinks: Array,
    }
}
</script>

<template>
    <footer>
        <div class="links-foot container-fluid">
            <div class="row row-cols-4">
                <div class="col logo-foot">
                <div class="p-3">
                    <img :src="logo.img" :alt="logo.nameLogo">
                </div>
                </div>
                <div class="col links-foot">
                <div class="p-3 text-uppercase">
                    <h4>quick links</h4>

                    <div class="line-green">
                        <div class="lineOne"></div>
                        <div class="lineTwo"></div>
                    </div>

                    <ul class="links p-0">
                        <li class="m-0" v-for="link in quickLinks">
                            <a href="#">{{ link }}</a>
                        </li>
                    </ul>
                </div>
                </div>
                <div class="col contacts-foot">
                <div class="p-3">Row column</div>
                </div>
                <div class="col map-foot">
                <div class="p-3">Row column</div>
                </div>
            </div>
</div>
    </footer>
</template>

<style lang="scss" scoped>
ul{
    list-style: none;
}
</style>