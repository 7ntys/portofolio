<script>
import AboutMeContent from "@/components/AboutMeContent.vue";

export default {
  name: "AboutMe",
  components: {AboutMeContent},
  data() {
    return {
      hovering: "container"
    };
  }
}
</script>

<template>
  <div class="about-container">
    <h2>Get to know me</h2>
    <div class="photo-container">
      <div class="container">
        <img src="../assets/Julien.png" alt="Julien Le Ber" />
      </div>
      <div class="photo-content">
        <AboutMeContent title="Level" content="Student" :img-path="require('../assets/diploma.png')" :img-hover-path="require('../assets/diplomaHover.png')"/>
        <AboutMeContent title="Level" content="Student" :img-path="require('../assets/diploma.png')"/>
        <AboutMeContent title="Level" content="Student" :img-path="require('../assets/diploma.png')"/>
      </div>
    </div>
  </div>
</template>

<style scoped lang="css">
.photo-container{
  position: relative;
  display: grid;
  grid-template-columns: 50% 50%;
  align-items: center;
  margin: 15%;
}
img{
  width: 100%;
  height: auto;
  border-radius: 20px;
}
.photo-content{
  width: 100%;
  display: grid;
  grid-template-columns: 30% 30% 30%;
  justify-content: space-around;
}

.container {
  --border-width: 3px;

  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 400px;
  height: 400px;
  font-family: Lato, sans-serif;
  font-size: 2.5rem;
  text-transform: uppercase;
  color: white;
  background: #222;
  border-radius: var(--border-width);

  &::after {
    position: absolute;
    content: "";
    top: calc(-1 * var(--border-width));
    left: calc(-1 * var(--border-width));
    z-index: -1;
    width: calc(100% + var(--border-width) * 2);
    height: calc(100% + var(--border-width) * 2);
    background: linear-gradient(
        60deg,
        hsl(224, 85%, 66%),
        hsl(269, 85%, 66%),
        hsl(314, 85%, 66%),
        hsl(359, 85%, 66%),
        hsl(44, 85%, 66%),
        hsl(89, 85%, 66%),
        hsl(134, 85%, 66%),
        hsl(179, 85%, 66%)
    );
    background-size: 300% 300%;
    background-position: 0 50%;
    border-radius: calc(2 * var(--border-width));
    animation: moveGradient 4s alternate infinite;
  }
}

@keyframes moveGradient {
  50% {
    background-position: 100% 50%;
  }
}

</style>