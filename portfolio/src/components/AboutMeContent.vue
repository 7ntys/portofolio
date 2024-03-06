<script>
export default {
  name: "AboutMeContent",
  props: ["title","content","imgPath","imgHoverPath"],
  data(){
    return{
      hovering: false
    }
  }
}
</script>

<template>
  <div class="content-container" @mouseenter="hovering=true" @mouseleave="hovering=false">
    <img :src="hovering ? imgHoverPath : imgPath">
    <h3>{{title}}</h3>
    <p>{{content}}</p>
  </div>
</template>

<style scoped>
.content-container{
  width: 100%;
  border-radius: 20px;
  background-color: #11D9C5;
  margin: 0 10px;
  border: #011126 solid 2px;
  transition: ease 0.5s;
}
img{
  width:51px;
  height: auto;
  transition: ease 0.5s;
}
.content-container:hover{
  background-color: #011126;
  color: #11D9C5;
  border: #11D9C5 solid 2px;
  transition: ease 0.5s;
}
</style>