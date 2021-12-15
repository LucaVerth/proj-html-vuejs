<template>
  <main>
    <div class="main-container">
      <Jumbotron/>
      <WorkCulture/>
      <UpgradeLife/>
      <OnlineCourses/>
      <People/>
      <Transform/>
      <Blogs/>
      <Subscribe/>
    </div>
  </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue';
import WorkCulture from './WorkCultureSection.vue';
import UpgradeLife from './UpgradeLife.vue';
import OnlineCourses from './OnlineCourses.vue';
import People from './People.vue';
import Transform from './Transform.vue';
import Blogs from './Blogs.vue';
import Subscribe from './Subscribe.vue';

export default {
  name: 'Main',
  components: {
    Jumbotron,
    WorkCulture,
    UpgradeLife,
    OnlineCourses,
    People,
    Transform,
    Blogs,
    Subscribe,
  }
}
</script>

<style lang="scss">
.main-container {
  height: calc(100% - 630px);
}
</style>