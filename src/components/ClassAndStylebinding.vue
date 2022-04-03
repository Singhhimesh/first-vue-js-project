<template>
  <div>
    <h2 v-bind:style="{ color: 'blue' }">Style binding</h2>
    <h1 v-bind:class="{ display: true }">Class binding obeject</h1>
    <h1 class="home">Class and style binding</h1>
  </div>
</template>

<script>
export default {
  name: "StyleBinding",
};
</script>

<style>
.home {
  background: red;
  color: white;
  font-family: cursive;
}
</style>