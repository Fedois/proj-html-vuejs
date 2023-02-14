<script>
import AppHeader from './components/componentsHeader/AppHeader.vue'
import AppMain from './components/componentsMain/AppMain.vue'
import AppFooter from './components/componentsFooter/AppFooter.vue'


export default {
  name: 'app',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
  data (){
    return {
      phoneOne: '(001) 88451234',
      phoneTwo: '88455438',
      logo: {
        img: '/src/assets/cropped-Group-39-2x.png',
        nameLogo: 'Phlox | Business'
      },
      
      icons: [
        {
          icon: 'fa-brands fa-facebook-f',
          nameIcon: 'facebook'
        },
        {
          icon: 'fa-brands fa-twitter',
          nameIcon: 'twitter'
        },
        {
          icon: 'fa-brands fa-pinterest-p',
          nameIcon: 'pinterest'
        },
      ],
      
      listNav: ['home', 'about', 'service', 'showcase', 'blog', 'contact'],
      quickLinks: ['carreers', 'news', 'terms of use', 'privacy projects', 'about', 'contact'],
      contacts: [
        {
          street: 'Patricia C. Amedee 4401 Waldeck Street grapevine nashville, TX 76051',
          email: 'info@yourdomain.com',
          number: '+99 (0) 101 0000 888'
        }
      ],
      map: '/src/assets/map.png'
    }
  }
}
</script>

<template>
  <AppHeader 
    :numOne="phoneOne"
    :numTwo="phoneTwo" 
    :icons="icons"
    :logo="logo"
    :linkNav="listNav"/>
  
  <AppMain />
  
  <AppFooter
  :logo="logo"
  :quickLinks="quickLinks"
  :contacts="contacts"
  :map="map"
  :icons="icons" />
</template>

<style lang="scss">
@use "./main.scss";
</style>
