<template>
  <div>
    <div class="main">
      <div class="footerSections">
        <h3>Get Started</h3>
        <p>Carrers</p>
        <p>Blog</p>
      </div>
      <div class="footerSections">
        <h3>Grow Toghter</h3>
        <p>Partners with Rodeo</p>
      </div>
      <div class="footerSections">
        <h3>Contact</h3>
        <p>Contact Us</p>
      </div>
      <div class="footerSections">
        <h3>Privacy Policy</h3>
        <p>Privacy Policy</p>
      </div>
      <div class="footerSections">
        <img src="../assets/images/Rodeo logo.png" alt="" />
        <div class="icons">
          <i class="fa-brands fa-linkedin-in"></i>
          <i class="fa-brands fa-instagram"></i>
          <i class="fa-brands fa-tiktok"></i>
        </div>
      </div>
    </div>
    <div class="footer">
      <p>CopyRight 2022 Rodeo Secure Inc.All Rights Are Reserved</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterEnd",
};
</script>

<style scoped>
.main {
  background: #70ffe5;
  display: flex;
  justify-content: space-between;
  padding: 2rem 4rem;
}
.icons i {
  margin: 5px 1%;
  background: #4f085e;
  color: white;
  padding: 5px;
  border-radius: 15px;
}
.footer {
  text-align: center;
  background: #4f085e;
  color: white;
  padding: 10px;
}
.footer p {
  margin-top: 10px;
}
@media (max-width: 768px) {
  .main {
    display: block;
  }
}
</style>
