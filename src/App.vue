<template>
  <div id="app">{{ user.username }}</div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      followers: 0,
      user: {
        id: 1,
        username: "suagrvoid",
        firstName: "mark",
        lastName: "brown",
        email: "email.com",
        isAdmin: true
      }
    };
  },
  computed: {
    fullName() {
      return `${this.user.firstName}`;
    }
  }
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
