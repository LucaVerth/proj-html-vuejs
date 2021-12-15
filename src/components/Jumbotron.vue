<template>
  <section class="jumbotron container-fluid">
    <figure class="jumbotron-image">
      <img
        :src="require('../assets/images/home-3-hero-bg.jpg')"
        alt="Jumbotron image"
      />
      <div class="jumbotron-center-section">
        <h3 class="fw-bold">Commence Business</h3>
        <h1>Distant Mentoring Program</h1>
        <a class="btn btn-custom mt-4" href="#" role="button"
          >Download free guidebook &#8594;
        </a>
      </div>
      <div class="jumbotron-favicons rounded-start">
        <i class="fas fa-ruler-vertical"></i>
        <i class="far fa-life-ring"></i>
        <i class="fas fa-book"></i>
        <i class="fas fa-shopping-cart"></i>
      </div>
    </figure>
  </section>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';

.jumbotron {
  margin: unset;
  padding: unset;
  max-height: 700px;
  .jumbotron-image {
    position: relative;
    .jumbotron-center-section {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 40%;
      height: 300px;
      color: #ffff;
      .btn-custom{
        padding: 13px 40px;
        background-color: #ffff;
        color: $secondary-color;
        transition: all 0.2s ease-in-out;
        &:hover{
          background-color: $secondary-color;
          color: #ffff;
        }
      }
      h1{
        font-size: 50px;
      }
    }
    .jumbotron-favicons{
      position: absolute;
      right: 0;
      top: 15%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-evenly;
      width: 40px;
      height: 150px;
      background-color: #ffff;
      i{
        padding: 0.5rem 0;
        cursor: pointer;
        opacity: 0.8;
      }
    }
    img {
      max-width: 100%;
    }
  }
}
</style>
