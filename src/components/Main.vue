<template>
  <main>
    <div class="main-container">
      <Jumbotron/>
      <WorkCulture/>
      <UpgradeLife/>
    </div>
  </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue';
import WorkCulture from './WorkCultureSection.vue';
import UpgradeLife from './UpgradeLife.vue';

export default {
  name: 'Main',
  components: {
    Jumbotron,
    WorkCulture,
    UpgradeLife,
  }
}
</script>

<style lang="scss">
main{
  height: calc(100vh - 80px);
}
</style>