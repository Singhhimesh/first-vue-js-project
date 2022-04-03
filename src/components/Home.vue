<template>
  <h1>Hello from home components</h1>
  <!-- <h1>Name is => {{ name }}</h1>
    <h2 v-if="show">Condition statements here</h2>
    <h1 v-else>else part will be executed</h1>
    <button v-on:click="hello('Suraj Kashyap')">Click</button> -->
  <center>
    <table border="1" cellpadding="5" cellspacing="0">
      <tr>
        <th>ID</th>
        <th>Name</th>
        <th>Phone</th>
        <th>Email</th>
        <th>Action</th>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.phone }}</td>
        <td>{{ user.email }}</td>
        <td>
          <button>Edit</button>
          <button style="margin-left: 5px">Delete</button>
        </td>
      </tr>
    </table>
  </center>
</template>

<script>
export default {
  name: "HomeComponent",
  props: {
    name: String,
  },
  data() {
    return {
      users: [
        {
          id: 1,
          name: "Suraj Kashyap",
          phone: "9315981404",
          email: "surajkashyayp9911@gmail.com",
        },
        {
          id: 2,
          name: "Akash Kashyap",
          phone: "9911993618",
          email: "akashkashyap9911@gmail.com",
        },
        {
          id: 3,
          name: "Laxmi Kashyap",
          phone: "9953097847",
          email: "laxmikumari@gmail.com",
        },
      ],
    };
  },
  methods: {
    hello(data) {
      console.log(data);
      this.show = !this.show;
    },
  },
};
</script>
