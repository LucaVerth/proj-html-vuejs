<template>
  <main>
    <div class="main-container">
      <Jumbotron/>
      <WorkCulture/>
    </div>
  </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue';
import WorkCulture from './WorkCultureSection.vue';

export default {
  name: 'Main',
  components: {
    Jumbotron,
    WorkCulture,
  }
}
</script>

<style lang="scss">
main{
  height: calc(100vh - 80px);
}
</style>