<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 main-section">
          <div class="image-mosaic">
            <img
              class="image1"
              :src="require('../assets/images/home-3-team-image.png')"
              alt=""
            />
            <img
              class="image2"
              :src="require('../assets/images/maxcoach-shape-05.png')"
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
              :src="require('../assets/images/maxcoach-shape-01.png')"
              alt=""
            />
            <img
              class="image6"
              :src="require('../assets/images/circle.png')"
              alt=""
            />
          </div>
          <div class="text-side">
            <div>
              <span class="slogan text-uppercase">everything in maxcoach</span>
              <h2 class="my-3">
                We're Here to<span class="transform"> Transform</span> You!
              </h2>
              <p>
                As learners, people can enjoy great companionship from MaxCoach mentors and educators. We can help you develop and grow at your best.
              </p>
              <a class="btn custom-btn mt-4" href="#">Get Free Guide</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Transform",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
section {
  background-color: #ffff;
  padding-bottom: 100px;
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
    .transform{
      color: $secondary-color;
      font-family:'Times New Roman', Times, serif;
      font-weight: bold;
    }
    h2 {
      font-size: 50px;
    }
    p{
      color: $text-style;
    }
    .custom-btn{
      background-color: $secondary-color;
      color: #ffff;
      padding: 10px 35px;
      transition: all 0.2s ease-in-out;
      &:hover{
        background-color: $grey-style;
        color: $secondary-color;
      }
    }
  }
  .image-mosaic {
    width: 50%;
    position: relative;
    margin-right: 10%;
    .image1 {
      position: absolute;
      top: 50%;
      right: 10%;
      transform: translate(20%, -50%);
      border-radius: 5px;
      z-index: 3;
    }
    .image2 {
      position: absolute;
      top: 145px;
      left: 6%;
      z-index: 2;
    }
    .image3 {
      position: absolute;
      top: 10%;
      left: 115px;
      opacity: 0.4;
      filter: invert(54%) sepia(56%) saturate(453%) hue-rotate(121deg)
        brightness(92%) contrast(95%);
    }
    .image4 {
      position: absolute;
      bottom: -105px;
      right: 19%;
    }
    .image5 {
      position: absolute;
      bottom: 5%;
      left: -150px;
      z-index: 4;
    }
    .image6{
      position: absolute;
      top: -30px;
      right: -23%;
      border-radius: 5px;
      z-index: 3;
      width: 50px;
      opacity: 0.7;
    }
  }
}
</style>
