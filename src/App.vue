<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <pro-suraj v-bind:name="userName" />
  <style-binding />
  <my-component />
</template>

<script>
// import Home from "./components/Home.vue";
// import MyComponent from "./components/mycom.vue";
// import StyleBinding from "./components/ClassAndStylebinding.vue";
import ProSuraj from "./components/Property.vue";

export default {
  name: "App",
  components: {
    // Home,
    // MyComponent,
    // StyleBinding,
    ProSuraj,
  },
  data() {
    return { userName: "Akash Kashyap" };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
