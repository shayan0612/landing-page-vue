<template>
  <div>
    <div class="container1">
      <div class="image">
        <img src="../assets/images/Rodeo logo.png" />
      </div>
      <div>
        <b-navbar toggleable="lg" class="nav-top">
          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

          <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav> </b-navbar-nav>

            <b-navbar-nav class="ml-auto">
              <b-nav-form class="links">
                <div class="nav-link">
                  <a href="/get">Get Started</a>
                  <a href="#">Education Center</a>
                  <a href="#">About Us</a>
                  <a href="#">Privacy Policy</a>
                  <b-button class="btn-sign">Sign In</b-button>
                </div>
              </b-nav-form>
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "NavBar",
};
</script>
<style scoped>
.container1 {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 1rem;
  padding: 10px 3rem;
}
.nav-link {
  display: flex;
}
.links a {
  margin-right: 3rem;
  text-decoration: none;
  color: #6c0755;
  font-weight: 700;
  font-size: 20px;
  line-height: 20px;
}
.btn-sign {
  border-radius: 1.25rem;
  color: #fd4cb7;
  background: #e3fd83;
  border: none;
}

@media (max-width: 992px) {
  .nav-link {
    flex-direction: column;
  }
  .links a {
    margin: 0;
  }
  .nav-top {
    justify-content: end;
    display: block;
  }
}
/* @media (min-width: 992px) {
  .container {
    max-width: 1030px;
  }
} */
</style>
