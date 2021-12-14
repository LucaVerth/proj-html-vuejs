<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 top-half">
          <div class="text-side">
            <div>
              <span class="slogan text-uppercase">everything in maxcoach</span>
              <h2 class="my-3 ">Learn about our <span class="fw-light">Work Culture</span> at MaxCoach</h2>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi dolor tempore odit mollitia ducimus exercitationem illo voluptates repudiandae, ea, explicabo cupiditate! Dolore, officia corporis laudantium maiores impedit eum ipsa. Eligendi.</p>
              <span>Have questions? <a href="#">Get Free Guide &#8594;</a> </span>
            </div>
          </div>
          <div class="image-mosaic">
            <img class="image1" :src="require('../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg')" alt="" />
            <img class="image2" :src="require('../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg')" alt="" />
            <img class="image3" :src="require('../assets/images/maxcoach-shape-07.png')" alt="">
            <img class="image4" :src="require('../assets/images/maxcoach-shape-02.png')" alt="">
            
          </div>
        </div>
        <div class="col-12 bottom-half">
          <div class="stats">129+
            <span>ENROLLED LEARNERS</span>
          </div>
          <div class="stats">80
            <span>FINISHED SESSIONS</span>
          </div>
          <div class="stats">4%
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
.top-half {
  display: flex;
  margin-top: 80px;
  margin-bottom: 60px;
  .text-side {
    display: flex;
    justify-content:start;
    align-items: center;
    width: 40%;
    min-height: 500px;
    h2{
      font-size: 50px;
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
    .image3{
      position: absolute;
      top: -10px;
      right: 110px;
      border-radius: 5px;
      z-index: 1;
    }
    .image4{
      position: absolute;
      bottom: -20px;
      right: 20%;
      border-radius: 5px;
      z-index: 4;
    }
  }

}
.bottom-half{
  display: flex;
  justify-content: space-evenly;
  text-align: center;
  .stats{
    display: flex;
    flex-direction: column;
    margin: 0 -100px;
    font-size: 2.3rem;
    font-weight: bold;
    span{
      padding-top: 10px;
      font-size: 1rem;
      font-weight: normal;
    }
  }
}
</style>
