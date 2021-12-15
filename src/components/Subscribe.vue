<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 main-section">
          <div class="Subscribe">
            <h4>Subscribe <span class="sub-email">Newsletters</span></h4>
            <p>
              Enter your email address to register to our newsletter
              subscription delivered on a regular basis!
            </p>
            <div class="input-group m-4 search_bar">
              <input
                type="text"
                class="form-control"
                placeholder="Enter your email!"
              />
              <button
                class="btn custom-btn"
                type="button"
              >
                Subscribe
              </button>
            </div>
            <img
              class="image1"
              :src="require('../assets/images/maxcoach-shape-08.png')"
              alt=""
            />
            <img
              class="image2"
              :src="require('../assets/images/maxcoach-shape-02.png')"
              alt=""
            />
            <img
              class="image3"
              :src="require('../assets/images/circle.png')"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Subscribe",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
section {
  padding: 80px 0;
  background-color: #ffff;
}
.main-section {
  display: flex;
  justify-content: center;
  position: relative;
  .Subscribe {
    width: 45%;
    display: flex;
    align-items: center;
    flex-direction: column;
    text-align: center;
    h4 {
      font-size: 50px;
    }
    p {
      padding-top: 15px;
      color: $text-style;
    }
    .sub-email{
      color: $secondary-color;
      font-family:'Times New Roman', Times, serif;
      font-weight: bold;
    }
    .search_bar{
      input,
      button {
        padding: 0.8rem;
        background-color: $grey-style;
        border: none;
      }
      .custom-btn{
        background-color: $secondary-color;
        color: #ffff;
        border-left: 1px solid $secondary-color;
        &:hover{
          background-color: $grey-style;
          color: $secondary-color;
        }
      }
    }
    .image1 {
      position: absolute;
      width: 150px;
      height: 150px;
      top: 0px;
      right: 65px;
      border-radius: 5px;
      z-index: 1;
      transform: rotate(30deg)
    }
    .image2 {
      position: absolute;
      bottom: 40px;
      right: 5%;
      border-radius: 5px;
      z-index: 2;
      transform: rotate(10deg)
    }
    .image3{
      position: absolute;
      top: 40%;
      left: -3%;
      border-radius: 5px;
      z-index: 3;
      width: 60px;
      opacity: 0.6;
      filter: invert(48%) sepia(77%) saturate(368%) hue-rotate(121deg) brightness(101%) contrast(88%);
    }
  }
}
</style>
