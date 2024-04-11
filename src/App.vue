<template>
  <HeaderComponent />
  <MainComponent />
  <TopFooter />
  <MainFooter />
  <BottomFooter />
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue'
  import MainComponent from './components/MainComponent.vue'
  import TopFooter from './components/FooterComponents/TopFooter.vue'
  import MainFooter from './components/FooterComponents/MainFooter.vue'
  import BottomFooter from './components/FooterComponents/BottomFooter.vue'
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      TopFooter,
      MainFooter,
      BottomFooter
    }
  }
</script>

<style lang="scss" scoped>

</style>