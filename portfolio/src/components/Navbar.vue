<script>
export default {
  name: "NavbarComponent"
}
</script>

<template>
  <div class="nav-container">
    <p>Home</p>
    <p>About Me</p>
    <p>Projects</p>
    <p>Contact</p>
  </div>
</template>

<style scoped>
  .nav-container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 60px;
    padding: 0;
    background: #011126;
  }
  .nav-container p {
    margin: 10px;
    color: #11D9C5;
    font-family: "Lato", sans-serif;
    font-weight: 900;
    font-style: normal;
    cursor: pointer;
    font-size: 22px;
  }

</style>