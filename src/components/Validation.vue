<template>
  <div>
    <p v-if="error.length">
      <b>Please correct the following errors </b>
    </p>

    <ul>
      <li v-for="e in error" v-bind:key="e.id">
        {{ e }}
      </li>
    </ul>
    <form @submit="login">
      <input type="text" placeholder="enter name" v-model="name" /><br /><br />
      <input
        type="password"
        placeholder="enter password"
        v-model="password"
      /><br /><br />
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Validation",
  data() {
    return {
      error:[],
      name: null,
      password: null,
    };
  },
  methods: {
    login(e) {
      this.error = [];
      if (this.name && this.password) {
        console.warn("no error");
      }
      if (!this.name) {
      this.error.push("Username required");
      }
      if (!this.password) {
     this.error.push("Password Required");
      }

      console.warn("Hello",this.error);
      e.preventDefault();
    },
  },
};
</script>