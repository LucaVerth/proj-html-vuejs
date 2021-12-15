<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 top-half">
          <div class="text-side">
            <div>
              <span class="slogan text-uppercase">everything in maxcoach</span>
              <h2 class="my-3">
                Learn about our <span class="work">Work Culture</span> at
                MaxCoach
              </h2>
              <p>
                Spend some time to visit our website or head office and discover our current courses, enrollment procedure, and registration deadline. We're opening new classes every beginning of each month.
              </p>
              <span
                >Have questions? <a class="work-link" href="#">Get Free Guide &#8594;</a>
              </span>
            </div>
          </div>
          <div class="image-mosaic">
            <img
              class="image1"
              :src="
                require('../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg')"
              alt=""
            />
            <img
              class="image2"
              :src="
                require('../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg')
              "
              alt=""
            />
            <img
              class="image3"
              :src="require('../assets/images/maxcoach-shape-07.png')"
              alt=""
            />
            <img
              class="image4"
              :src="require('../assets/images/maxcoach-shape-02.png')"
              alt=""
            />
            <img
              class="image5"
              :src="require('../assets/images/circle.png')"
              alt=""
            />
          </div>
        </div>
        <div class="col-12 bottom-half">
          <div class="stats">
            129+
            <span>ENROLLED LEARNERS</span>
          </div>
          <div class="stats">
            80
            <span>FINISHED SESSIONS</span>
          </div>
          <div class="stats">
            4%
            <span>SATISFACTION RATE</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "WorkCultureSection",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
section {
  margin-bottom: 110px;
}
.top-half {
  display: flex;
  margin-top: 80px;
  margin-bottom: 60px;
  .text-side {
    display: flex;
    justify-content: start;
    align-items: center;
    width: 40%;
    min-height: 500px;
    .work{
      color: $secondary-color;
      font-family:'Times New Roman', Times, serif;
      font-weight: bold;
    }
    .work-link{
      color: $secondary-color;
    }
    h2 {
      font-size: 50px;
    }
    p{
      color: $text-style;
    }
  }
  .image-mosaic {
    width: 60%;
    position: relative;
    .image1 {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      border-radius: 5px;
      z-index: 2;
    }
    .image2 {
      position: absolute;
      top: -20px;
      right: 25px;
      border-radius: 5px;
      z-index: 3;
    }
    .image3 {
      position: absolute;
      top: -10px;
      right: 110px;
      border-radius: 5px;
      z-index: 1;
    }
    .image4 {
      position: absolute;
      bottom: -20px;
      right: 20%;
      border-radius: 5px;
      z-index: 4;
    }
    .image5{
      position: absolute;
      top: 50px;
      left: -20px;
      border-radius: 5px;
      z-index: 3;
      width: 50px;
      opacity: 0.7;
    }
  }
}
.bottom-half {
  display: flex;
  justify-content: space-evenly;
  text-align: center;
  .stats {
    display: flex;
    flex-direction: column;
    margin: 0 -100px;
    font-size: 2.3rem;
    font-weight: bold;
    color: $secondary-color;
    span {
      padding-top: 10px;
      font-size: 1rem;
      font-weight: normal;
      color: $primary-color;
    }
  }
}
</style>
