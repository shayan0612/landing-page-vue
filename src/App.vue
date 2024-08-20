<template>
  <div id="app">
    <NavBar />
    <HeroSection />
    <Cards />
    <Footer />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import HeroSection from "./components/HeroSection.vue";
import Cards from "./components/Cards.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    NavBar,
    HeroSection,
    Cards,
    Footer,
  },
};
</script>

<style scoped>
* {
  font-family: "League Spartan", sans-serif;
}
</style>
