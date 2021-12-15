<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 text-center blogs">
          <span class="text-uppercase">read for more joyment</span>
          <h2>Latest From <span class="blog">Our Blogs</span></h2>
        </div>
        <div class="col-12">
          <div class="">
            <div class="main-carousel">
              <div
                class="cards"
                v-for="(post, index) in BlogPosts"
                :key="index"
              >
                <a class="blog-links" href="#">
                  <img
                    class="rounded-top"
                    :src="require(`../assets/images/${post.image}`)"
                    alt=""
                  />
                </a>
                <div class="text">
                  <span class="post-type">{{ post.type.toUpperCase() }}</span>
                  <h5 class="mt-3">{{ post.title }}</h5>
                  <div class="extra-info mt-4">
                    <span class="me-3">
                      <i class="far fa-calendar"></i>
                      {{ post.date }}
                    </span>
                    <span class="ms-3">
                      <i class="far fa-eye"></i>
                      {{ post.views }} views
                    </span>
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
import BlogPosts from '../assets/data/BlogPosts.js';
export default {
  name: 'Blogs',
  data(){
    return{
      BlogPosts,
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
section{
  padding-top: 80px;
  margin-bottom: 100px;
}
.blogs {
  h2 {
    font-size: 50px;
    margin-top: 20px;
    margin-bottom: 60px;
  }
  .blog{
    color: $secondary-color;
    font-family:'Times New Roman', Times, serif;
    font-weight: bold;
  }
}
.main-carousel {
  display: flex;
  justify-content: space-between;
  .cards {
    width: 400px;
    min-height: 450px;
    border-radius: 10px;
    background-color: transparent;
    .text {
      padding: 20px 0;
      .post-type{
        color: $dark-grey-style;
      }
      .extra-info{
        color: $dark-grey-style;
      }
    }
    h5{
      line-height: 35px;
    }
  }
}
</style>