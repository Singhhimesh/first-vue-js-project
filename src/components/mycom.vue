<template>
  <div>
    <h1>Template in vue js</h1>
    <h3 v-once>{{ name }}</h3>
    <h3>{{ name }}</h3>
    <p v-html="rawHtml"></p>
    <h1>{{ a + b }}</h1>
    <h1>{{ ok ? "yes" : "no" }}</h1>
    <button v-bind:disabled="disabledBtn" v-on:click="Click()">Click Me</button>
  </div>
</template>

<script>
export default {
  name: "MyComponent",
  data() {
    return {
      name: "Suraj Kashyap",
      a: 10,
      b: 20,
      ok: true,
      rawHtml: "<h1>hello<h1>",
      disabledBtn:false
    };
  },
  methods: {
    Click() {
      this.name = "Suraj Singh";
      this.ok = !this.ok;
    },
  },
};
</script>