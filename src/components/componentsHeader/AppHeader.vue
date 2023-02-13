<script>
export default {
    name: 'AppHeader',
    data () {
        return {
            phoneOne: '(001) 88451234',
            phoneTwo: '88455438',
            listNav: ['home', 'about', 'service', 'showcase', 'blog', 'contact'],
            socials: [
                {
                    icon: 'fa-brands fa-twitter',
                    name: 'twitter'
                },
                {
                    icon: 'fa-brands fa-facebook-f',
                    name: 'facebook'
                },
                {
                    icon: 'fa-brands fa-pinterest-p',
                    name: 'pinterest'
                },
            ]
        }
    }
}
</script>

<template>
    <header>
         
    </header>
</template>

<style lang="scss" scoped>
.phone-number{
    background-color: black;
}
</style>