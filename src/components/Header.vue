<template>
  <header id="head" class="header">
    <div class="container-fluid custom_container">
      <div class="row custom_row">
        <nav class="col nav-bar">
          <ul class="nav">
            <li class="nav-item ms-2" v-for="(link, index) in linksHeader" :key="index">
              <a class="nav-link custom_link" :href="link.link"
                >{{link.title}}
                <i class="fas fa-chevron-down"></i>
              </a>
            </li>
          </ul>
        </nav>
        <figure class="col-3 logo-header">
          <img class :src="require('../assets/images/dark-logo.png')" alt="" />
        </figure>
        <div class="col search-bar">
          <a href="#"><i class="fas fa-shopping-cart"></i></a>
          <a href="#"><i class="far fa-user-circle mx-2"></i></a>
          <div class="input-group custom_search_bar">
            <input type="text" class="custom_search" placeholder="Search..." />
            <button class="btn custom_btn" type="button">
              <i class="fas fa-search"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import linksHeader from '../assets/data/LinksHeader.js';

export default {
  name: "Header",
  data(){
    return {
      linksHeader, 
    }
  }
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';

header {
  width: 100%;
  height: 80px;
  background-color: #fff;
  min-width: 1750px;
  overflow-x: hidden;
  .custom_container {
    width: 80%;
    margin: 0 auto;
  }
  .custom_row {
    height: 80px;
    justify-content: space-between;
    align-items: center;
    figure {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: unset;
      padding: unset;
      img {
        max-width: 50%;
        padding: 0.5em;
      }
    }
    .custom_link{
      padding: 0 0.6rem;
      &:hover{
        color: $secondary-color;
      }
    }
    .nav-bar ul li a {
      color: $primary-color;
      font-size: 1rem;
      i{
        font-size: 0.6rem;
        line-height: 40px;
      }
    }
    .search-bar {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      .custom_search_bar {
        width: unset;
      }
      .custom_search {
        width: 250px;
        padding: 10px;
        background-color: $grey-style;
        border-radius: 5px;
        border: 1px solid transparent;
      }
      .custom_btn {
        background-color: $grey-style;
        color: $secondary-color;
      }
      a {
        margin: 0.5em;
        text-decoration: none;
        i {
          cursor: pointer;
          font-size: 1.3rem;
          color: $dark-grey-style;
          &:hover{
            color: $secondary-color;
          }
        }
      }
    }
  }
}
</style>
