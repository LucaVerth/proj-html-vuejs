<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col-12 text-light footer_custom">
          <div class="address">
            <h5 class="fw-bold">Address</h5>
            <div>
              <ul class="address-list">
                <li>382 NE 191st St # 87394 Miami, FL 33179-3899</li>
                <li>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</li>
                <li>support@maxcoach.com</li>
              </ul>
            </div>
            <div class="social-links">
              <a href="#">
                <i class="fab fa-facebook-square"></i>
              </a>
              <a href="#">
                <i class="fab fa-twitter"></i>
              </a>
              <a href="#">
                <i class="fab fa-instagram"></i>
              </a>
              <a href="#">
                <i class="fab fa-linkedin"></i>
              </a>
            </div>
          </div>
          <div class="links">
            <div class="left-links">
              <h5 class="fw-bold">Explore</h5>
              <div class="links-container mt-2">
                <div class="item"><a href="#">Start Here</a></div>
                <div class="item"><a href="#">Blog</a></div>
                <div class="item"><a href="#">About Us</a></div>
                <div class="item"><a href="#">Success Story</a></div>
                <div class="item"><a href="#">Courses</a></div>
                <div class="item"><a href="#">Contact Us</a></div>
              </div>
            </div>
            <div class="right-links ps-5">
              <h5 class="fw-bold">Information</h5>
              <div class="links-container mt-2">
                <div class="item"><a href="#">Membership</a></div>
                <div class="item"><a href="#">Purchase guide</a></div>
                <div class="item"><a href="#">Privacy policy</a></div>
                <div class="item"><a href="#">Terms of service</a></div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 text-light copyright d-flex justify-content-center">
          <span>&copy; 2020 Maxcoach. All Rights Reserved</span>
        </div>
      </div>
    </div>
    <a class="top-page-button" href="#head">
      <i class="fas fa-arrow-up"></i>
    </a>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
@import '../assets/style/Vars.scss';
footer {
  height: 500px;
  background-color: #171520;
  position: relative;
  .top-page-button {
    position: absolute;
    right: 30px;
    bottom: 30px;
    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
      0 3px 1px -2px rgba(0, 0, 0, 0.2);
      background-color: #1fad95;
      color: #fff;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    text-align: center;
    font-size: 25px;
    line-height: 60px;
    cursor: pointer;
  }
  .copyright{
    span{
      color: $text-style;
    }
  }
}
.footer_custom {
  display: flex;
  justify-content: space-between;
  .address {
    width: 50%;
    padding: 70px 0;
  }
  .address ul {
    list-style-type: none;
    padding: 10px 0;
    li {
      padding: 10px 0;
      color: $text-style;
    }
  }
  .social-links {
    width: 35%;
    display: flex;
    justify-content: space-between;
    i {
      font-size: 1.8rem;
    }
    a {
      text-decoration: none;
      color: $text-style;
      &:hover{
        color: $secondary-color;
      }
    }
  }
  .links {
    width: 50%;
    padding: 70px 0;
    display: flex;
    justify-content: space-around;
    .left-links {
      display: flex;
      flex-direction: column;
      width: 50%;
      .links-container {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        max-height: 50%;
        div {
          width: 50%;
          padding: 8px 0;
          a {
            text-decoration: none;
            color: $text-style;
            &:hover{
              color: $secondary-color;
              text-decoration: underline;
            }
          }
        }
      }
    }
    .right-links {
      width: 50%;
      display: flex;
      flex-direction: column;
      .links-container {
        display: flex;
        flex-direction: column;
        div {
          width: 50%;
          padding: 8px 0;
          a {
            text-decoration: none;
            color: $text-style;
            &:hover{
              color: $secondary-color;
              text-decoration: underline;
            }
          }
        }
      }
    }
  }
}
</style>
