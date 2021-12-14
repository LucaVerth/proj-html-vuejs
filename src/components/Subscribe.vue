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
  background-color: green;
  .Subscribe {
    width: 45%;
    display: flex;
    align-items: center;
    flex-direction: column;
    text-align: center;
    background-color: red;
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
  }
}
</style>
