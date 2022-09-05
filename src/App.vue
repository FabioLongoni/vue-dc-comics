<template>
  <div id="app">
    <MainHeader />
    <MainContent />
    <FooterContent />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
import FooterContent from './components/FooterContent.vue';


export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    FooterContent,
}
}
</script>

<style lang="scss">
  @import './style/index';

</style>
