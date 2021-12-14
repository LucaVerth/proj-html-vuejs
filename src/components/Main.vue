<template>
  <main>
    <div class="main-container">
      <Jumbotron/>
      <WorkCulture/>
      <UpgradeLife/>
      <OnlineCourses/>
    </div>
  </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue';
import WorkCulture from './WorkCultureSection.vue';
import UpgradeLife from './UpgradeLife.vue';
import OnlineCourses from './OnlineCourses.vue';

export default {
  name: 'Main',
  components: {
    Jumbotron,
    WorkCulture,
    UpgradeLife,
    OnlineCourses,
  }
}
</script>

<style lang="scss">
main{
  height: calc(100vh - 80px);
}
</style>