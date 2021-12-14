<template>
  <main>
    <div class="main-container">
      <Jumbotron/>
    </div>
  </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue';

export default {
  name: 'Main',
  components: {
    Jumbotron,
  }
}
</script>

<style lang="scss" scoped>
main{
  height: calc(100% - 80px);
}
</style>