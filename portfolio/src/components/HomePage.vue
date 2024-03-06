<script>
import NavbarComponent from "@/components/Navbar.vue";
import AboutMe from "@/components/AboutMe.vue";

export default {
  name: "HomePage",
  components: {AboutMe, NavbarComponent}
}
</script>

<template>
  <div class="container">
    <NavbarComponent />
    <div class="home-container">
      <h1>Hi, I'm Julien Le Ber</h1>
      <p>I'm a student in Cybersecurity</p>
    </div>
    <div class="scroll-container">
      <p>Scroll down</p>
      <p class="scroll">↓</p>
    </div>
    <about-me />
  </div>
</template>

<style scoped>
.home-container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 90vh;
  color: #11D9C5;
  font-family: "Lato", sans-serif;
  font-weight: 900;
  font-style: normal;
}
.scroll-container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #11D9C5;
  font-family: "Lato", sans-serif;
  font-weight: 900;
  font-style: normal;
}
</style>