<template>
  <HeaderComponent />
  <MainComponent />
  <TopFooter />
  <MainFooter />
  <BottomFooter />
</template>

<script>
  import HeaderComponent from './assets/components/HeaderComponent.vue'
  import MainComponent from './assets/components/MainComponent.vue'
  import TopFooter from './assets/components/FooterComponents/TopFooter.vue'
  import MainFooter from './assets/components/FooterComponents/MainFooter.vue'
  import BottomFooter from './assets/components/FooterComponents/BottomFooter.vue'
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