<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 main-section">
          <div class="Subscribe">
            <h4>Subscribe Newsletters</h4>
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
                class="btn btn-success"
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
section {
  padding-top: 80px;
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
    }
    .search_bar{
      input,
      button {
        padding: 0.8rem;
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
  }
}
</style>
