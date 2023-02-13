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
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use "./main.scss";
</style>
