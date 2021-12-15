<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 text-center courses">
          <span class="text-uppercase">join maxcoach at best</span>
          <h2>Latest Online <span class="courses-text">Courses</span></h2>
        </div>
        <div class="col-12">
          <div class="carousel">
            <div class="main-carousel">
              <div
                class="cards"
                v-for="(card, index) in CardsToPrint"
                :key="index"
              >
                <a class="course-image" href="#">
                  <img
                    class="rounded-top"
                    :src="require(`../assets/images/${card.image}`)"
                    alt=""
                  />
                </a>
                <div class="text">
                  <span class="price-text">${{card.price.toFixed(2)}}</span>
                  <h5 class="mt-3">{{ card.title }}</h5>
                  <div class="extra-info mt-4">
                    <span class="me-3">
                      <i class="far fa-file-alt"></i>
                      {{ card.lessons }} Lessons
                    </span>
                    <span class="ms-3">
                      <i class="far fa-user"></i>
                      {{ card.students }} Students
                    </span>
                  </div>
                </div>
              </div>
            </div>
            <div class="carousel-dots text-center mt-3">
              <button class="active"></button>
              <button></button>
              <button></button>
              <button></button>
              <button></button>
            </div>
          </div>
        </div>
        <div class="col-6 offset-3 text-center courses-link mt-4">
          <p>
            Control your personal preferences settings to get notified about
            appropriate courses. <a class="link" href="#">View all courses &#8594;</a>
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import CardsToPrint from "../assets/data/Cards.js";

export default {
  name: "OnlineCourses",
  data() {
    return {
      CardsToPrint,
    };
  },
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
.courses {
  .courses-text{
    color: $secondary-color;
    font-family:'Times New Roman', Times, serif;
    font-weight: bold;
  }
  h2 {
    font-size: 50px;
    margin-top: 20px;
    margin-bottom: 60px;
  }
}
.main-carousel {
  display: flex;
  justify-content: space-between;
  .cards {
    width: 400px;
    min-height: 450px;
    border-radius: 10px;
    background-color: #fff;
    .text {
      padding: 20px;
      .price-text{
        color: $secondary-color;
        font-size: 1.5rem;
      }
      .extra-info{
        color: $dark-grey-style;
      }
    }
  }
}
.carousel-dots {
  button {
    background-color: $primary-color;
    opacity: 0.3;
    border-radius: 100%;
    width: 10px;
    height: 10px;
    border: none;
    margin: 15px;
    &.active {
      width: 15px;
      height: 15px;
      background-color: $primary-color;
      opacity: 1;
    }
  }
}
.courses-link {
  p {
    font-size: 1.2rem;
    color: $text-style;
  }
  .link{
    color: $primary-color;
  }
}
</style>
