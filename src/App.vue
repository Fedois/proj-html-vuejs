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
      listNav: ['home', 'about', 'service', 'showcase', 'blog', 'contact'],
      quickLinks: ['carreers', 'news', 'terms of use', 'privacy projects', 'about', 'contact'],
    }
  }
}
</script>

<template>
  <AppHeader 
    :numOne="phoneOne"
    :numTwo="phoneTwo" 
    :linkNav="listNav"/>
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use "./main.scss";

// general style
.my-button{
  border-radius: 50px;
  padding: 10px 30px;
  border: none
}
a{
  text-decoration: none;
}
</style>
