<template>
  <div>
    <h1>Hello from home components</h1>
    <h1>Name is => {{ name }}</h1>
    <h2 v-if="show">
        Condition statements here
    </h2>
    <h1 v-else>
        else part will be executed
    </h1>
    <button v-on:click="hello('Suraj Kashyap')">Click</button>
  </div>
</template>

<script>
export default {
  name: "HomeComponent",
  props: {
    name: String,
  },
  data() {
      return {
          show:true
      }
  },
  methods: {
    hello(data) {
        console.log(data);
        this.show = !this.show;
    },
  },
};
</script>
