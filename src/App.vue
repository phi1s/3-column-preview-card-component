<template>
  <!---<HelloWorld msg="Welcome to Your Vue.js App"/>--->
  <PreviewCard></PreviewCard>
</template>

<script>
import PreviewCard from "./components/PreviewCard.vue";

export default {
  name: "App",
  components: {
    PreviewCard,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@700&family=Lexend+Deca&display=swap");
@import "./assets/variables.css";
#app {
  font-family: "Big Shoulders Display", cursive;
  font-family: "Lexend Deca", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
