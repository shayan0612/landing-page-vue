<template>
  <!-- <b-container fluid="sm" class="head">
    <div class="content">
      <h1>Welcome to Rodeo Secure</h1>
      <h3>Custom Insurance Solution for CPG Brands</h3>
      <b-button class="btn-view">View Your Options</b-button>
    </div>
    <div class="container-img">
      <img src="../assets/images/hero.png" fluid alt="img" />
    </div>
  </b-container> -->
  <div class="position-relative">
    <div
      class="position-absolute h-100 left-0 top-0 justify-self-start main-container1"
    ></div>
    <div
      class="position-relative d-flex align-items-center justify-content-center container2"
    >
      <div>
        <h1 class="heading1">Welcome to Rodeo Secure</h1>
        <h3 class="heading3">Custom Insurance Solution for CPG Brands</h3>
        <b-button class="btn-view">View Your Options</b-button>
      </div>
      <img src="../assets/images/pinchtable 3 1.png" class="imageHero" />
    </div>
  </div>
</template>

<script>
export default {
  name: "HeroSection",
};
</script>
<style scoped>
.container1 {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 3rem;
}
.head {
  margin-top: 2.5rem;
  /* padding: 5rem 0; */
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: space-between;
}
.container-img {
  width: 30%;
  position: relative;
  right: 14rem;
}
.btn-view {
  border-radius: 1.25rem;
  color: #fd4cb7;
  background: #e3fd83;
  border: none;
}
.content1 {
  background: linear-gradient(249.17deg, #c7c8ff -0.42%, #9bfce6 100%);
  padding: 9rem 6.75rem;
  width: 70%;
  border-radius: 0 10px 10px 0;
  margin-bottom: 10px;
}
.heading1 {
  font-weight: 700;
  font-size: 80px;
  line-height: 80px;
}
.heading3 {
  font-weight: 700;
  font-size: 40px;
  line-height: 40px;
  color: #4f085e;
}
.container-img img {
  height: 28rem;
}
.imageHero {
  width: 50%;
}
.main-container1 {
  background: linear-gradient(249.17deg, #c7c8ff -0.42%, #9bfce6 100%);
  width: 70%;
  border-radius: 0 10px 10px 0;
  margin-bottom: 10px;
  z-index: 10;
}
.container2 {
  padding: 9rem 6.75rem;
  z-index: 50;
}
@media (max-width: 992px) {
  .main-container1 {
    width: 100%;
  }
  .container2 {
    display: block !important;
  }
  .imageHero {
    display: flex;
    margin: 20px auto;
    width: 100%;
  }
  .heading1 {
    font-size: 75px;
  }
}
@media (max-width: 600px) {
  .heading1 {
    font-size: 40px;
    line-height: 30px;
  }
  .heading3 {
    font-size: 25px;
    line-height: 25px;
  }
}
</style>
