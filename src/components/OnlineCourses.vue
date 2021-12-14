<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 text-center">TITLE TITLE</div>
        <div class="col-12">
          <div class="carousel">
            <div class="main-carousel">
              <div class="cards">CARD 1</div>
              <div class="cards">CARD 2</div>
              <div class="cards">CARD 3</div>
            </div>
            <div class="carousel-dots text-center mt-3"> : : : </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "OnlineCourses",
};
</script>

<style lang="scss" scoped>
.main-carousel{
  display: flex;
  justify-content: space-between;
  background-color:purple;
  .cards{
    width: 400px;
    background-color: red;
    border: 1px solid black;
  }
}
</style>
