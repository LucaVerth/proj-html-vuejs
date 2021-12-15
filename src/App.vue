<template>
  <div id="app">
    <div class="main-wrapper">
      <Header/>
      <Main/>
      <Footer/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/Generals.scss';
@import './assets/style/Vars.scss';

.main-wrapper{
  width: 100%;
  min-width: 1750px;
  overflow-x: hidden;
}

</style>
