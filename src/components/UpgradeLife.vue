<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 main-section">
          <div class="image-mosaic">
            <img
              class="image1"
              :src="require('../assets/images/stock-full-hd-11-670x450.jpg')"
              alt=""
            />
            <img
              class="image2"
              :src="require('../assets/images/maxcoach-shape-05-150x150.png')"
              alt=""
            />
            <img
              class="image3"
              :src="require('../assets/svg/svg-0.svg')"
              alt=""
            />
            <img
              class="image4"
              :src="require('../assets/images/maxcoach-shape-07-150x150.png')"
              alt=""
            />
            <img
              class="image5"
              :src="require('../assets/images/icon-youtube-play.png')"
              alt=""
            />
          </div>
          <div class="text-side">
            <div>
              <span class="slogan text-uppercase">how we work</span>
              <h2 class="my-3">
                Upgrade Your Skills<span class="upgrade">
                  Upgrade Your Life</span
                >
              </h2>
              <p>
                Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets of insights into your career. MaxCoach accompany learners in every stage of learning.
              </p>
              <span><a class="upgrade-link" href="#">Download free guidebook &#8594;</a> </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "UpgradeLife",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
section{
  margin-bottom: 100px;
}
.main-section {
  display: flex;
  margin-bottom: 60px;
  .text-side {
    display: flex;
    justify-content: start;
    align-items: center;
    width: 30%;
    min-height: 500px;
    .upgrade{
      color: $secondary-color;
      font-family:'Times New Roman', Times, serif;
      font-weight: bold;
    }
    .upgrade-link{
      color: $primary-color;
    }
    h2 {
      font-size: 50px;
    }
    p{
      color: $text-style;
    }
  }
  .image-mosaic {
    width: 50%;
    position: relative;
    margin-right: 10%;
    .image1 {
      position: absolute;
      top: 50%;
      left: 0;
      transform: translate(0, -50%);
      border-radius: 5px;
      z-index: 3;
    }
    .image2 {
      position: absolute;
      top: 90px;
      left: -15%;
      z-index: 2;
    }
    .image3 {
      position: absolute;
      top: -10%;
      left: -55px;
      opacity: 0.1;
    }
    .image4 {
      position: absolute;
      bottom: -35px;
      right: -3%;
    }
    .image5 {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 4;
    }
  }
}
</style>
