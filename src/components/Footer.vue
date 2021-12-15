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
          <div class="links">LINKS</div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
footer {
  height: 550px;
  background-color: #171520;
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
    & li {
      padding: 10px 0;
    }
  }
  .social-links {
    width: 35%;
    display: flex;
    justify-content: space-between;
    & i {
      font-size: 1.8rem;
    }
    a{
      text-decoration: none;
      color: #fff;
    }
  }
  .links {
    width: 50%;
    padding: 70px 0;
  }
}
</style>
