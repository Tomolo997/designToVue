<template>
  <main class="main-container">
    <Navbar />
    <LandingSection />
  </main>
</template>

<script>
import Navbar from "./components/Header/Navbar.vue";
import LandingSection from "./components/LandingSection/LandingSection.vue";
export default {
  name: "App",
  components: {
    Navbar,
    LandingSection,
  },
  data() {
    return {
      year: new Date().getFullYear(),
    };
  },
};
</script>

<style scoped>
</style>