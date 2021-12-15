<template>
  <section>
    <div class="custom-shape-divider-top-1639503039">
      <svg
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path
          d="M0,0V7.23C0,65.52,268.63,112.77,600,112.77S1200,65.52,1200,7.23V0Z"
          class="shape-fill"
        ></path>
      </svg>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-12 top-half">
          <div class="text-side">
            <div>
              <span class="slogan text-uppercase">testimonials</span>
              <h2 class="my-3">
                Why Do People <span class="hearts">*Hearts*</span> Us?
              </h2>
              <p>
                Seeking for verbals of our service quality? Find them here. Everything is transparent and straightforward for your sense of jusitifcation.
              </p>
              <span><a class="link" href="#">View all &#8594;</a> </span>
            </div>
          </div>
          <div class="image-carousel">
            <div class="cards">
              <div class="main-card">
                <div class="card-item item1">
                  <div class="text">
                    <h4 class="mb-3">
                      Professional Team of specialists and passionate mentors at
                      reach
                    </h4>
                    <div class="inner-content">
                      <p>
                       I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.	
                      </p>
                      <div class="profile mt-4">
                        <img
                          class="profile-image"
                          src="../assets/images/testimonial-avata-01.jpg"
                          alt=""
                        />
                        <div class="profile-info">
                          <h6>Madley Pondor</h6>
                          <span>/IT Specialist</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="card-item item2">
                  <div class="text">
                    <h4 class="mb-3">
                      High level of efficiency and scientific teaching methods
                    </h4>
                    <div class="inner-content">
                      <p>
                        I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.
                      </p>
                      <div class="profile mt-4">
                        <img
                          class="profile-image"
                          src="../assets/images/testimonial-avata-02.jpg"
                          alt=""
                        />
                        <div class="profile-info">
                          <h6>Mina Hollace</h6>
                          <span>/Freelance</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="card-item item3">
                  <div class="text">
                    <h4 class="mb-3">
                      The MaxCoach team works really hard to ensure high level of quality
                    </h4>
                    <div class="inner-content">
                      <p>
                       I am happy with their arrangement of lessons and subjects. They reflect a scientific  investigation into effective methods to adopt.	
                      </p>
                      <div class="profile mt-4">
                        <img
                          class="profile-image"
                          src="../assets/images/testimonial-avata-03.jpg"
                          alt=""
                        />
                        <div class="profile-info">
                          <h6>Matt Jeorge</h6>
                          <span>/IT Director</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "People",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
section {
  position: relative;
  background-color: #ffff;
  padding-top: 100px;

  .custom-shape-divider-top-1639503039 {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
  }
  .custom-shape-divider-top-1639503039 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 80px;
  }
  .custom-shape-divider-top-1639503039 .shape-fill {
    fill: $grey-style;
  }
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
    margin-right: 80px;
    padding-right: 50px;
    .hearts{
      color: $secondary-color;
      font-family:'Times New Roman', Times, serif;
      font-weight: bold;
    }
    .link{
      color: $primary-color;
      &:hover{
        color: $secondary-color;
        transition: color 0.3s ease-out;
      }
    }
    h2 {
      font-size: 50px;
    }
    p{
      color: $text-style;
    }
  }
  .image-carousel {
    width: 60%;
    position: relative;
    //min-height: 650px;
    .main-card {
      margin: 150px 0;
      width: 100%;
      min-height: calc(650px / 2);
      position: relative;
      .card-item {
        height: inherit;
        position: relative;
        background-color: #fff;
        perspective: 1200px;
        box-shadow: 2px 2px 8px;
        .text {
          padding: 40px;
          position: relative;
        }
        p{
          color: $text-style;
        }
      }
      // carousel cards items
      .item1{
        position: relative;
        top: auto;
        left: auto;
        transform: translateY(0%) translateZ(0px) rotateX(0deg) scale(1) perspective(1px);
        z-index: 1;
        backface-visibility: hidden;
      }
      .item2{
        position: absolute;
        top: 0;
        left: 0;
        transform: translateY(50%) translateZ(-50px) rotateX(0deg) scale(0.8) perspective(1px);
        opacity: 0.6;
      }
      .item3{
        position: absolute;
        top: 0;
        left: 0;
        transform: translateY(-50%) translateZ(-50px) rotateX(0deg) scale(0.8) perspective(1px);
        opacity: 0.6;
      }
      .profile {
        display: flex;
        align-items: center;
        .profile-image {
          width: 70px;
          height: 70px;
          border-radius: 50%;
          margin-right: 20px;
        }
        .profile-info{
          span{
            color: $text-style;
          }
        }
      }
    }
  }
}
</style>
