<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 top-half">
          <div class="text-side">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit
              repudiandae sunt nostrum, magnam repellendus quam animi, quasi
              quae illum sit neque placeat voluptatibus unde nemo quis alias?
              Perferendis, vero harum. Lorem ipsum dolor, sit amet consectetur
              adipisicing elit. Quae, vero. Ipsa obcaecati, dolor necessitatibus
              quibusdam nemo aut dolorem consequatur eaque reprehenderit esse
              nisi natus aspernatur, sint magnam nulla sed facilis? Lorem ipsum
              dolor sit amet consectetur adipisicing elit. Beatae, molestiae
              optio inventore magni nulla illum dolor error sint placeat.
              Debitis minus nesciunt id maiores laborum ratione ullam aliquam.
              Consectetur, eius. Lorem ipsum dolor sit amet consectetur
              adipisicing elit. Nostrum repellat natus vero enim amet sequi
              iusto corporis, delectus ratione, architecto quo deserunt omnis
              explicabo, totam aliquam ducimus voluptatum dolor nemo?
            </p>
          </div>
          <div class="image-mosaic">
            <img class="image1" :src="require('../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg')" alt="" />
            <img class="image2" :src="require('../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg')" alt="" />
            <img class="image3" :src="require('../assets/images/maxcoach-shape-07.png')" alt="">
            <img class="image4" :src="require('../assets/images/maxcoach-shape-02.png')" alt="">
            
          </div>
        </div>
        <div class="col-12 bottom-half">BOTTOM SIDE</div>
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
section {
  background-color: red;
}
.top-half {
  display: flex;
  margin-top: 50px;
  .text-side {
    width: 40%;
    background-color: green;
    min-height: 500px;
  }
  .image-mosaic {
    width: 60%;
    background-color: purple;
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
      top: 0;
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
</style>
