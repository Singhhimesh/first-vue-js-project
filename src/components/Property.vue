<template>
  <h6 v-for="user in users" :key="user.name">
    {{ user.name }} -- {{ user.email }}
  </h6>
</template>

<script>
export default {
  name: "ProSuraj",
  props: ["users"],
};
</script>