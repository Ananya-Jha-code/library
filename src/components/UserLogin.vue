<template>
    <div class="login">
      <h2>User Login</h2>
      <form @submit.prevent="login">
        <div>
          <label for="username">Username:</label>
          <input type="text" v-model="username" id="username" required />
        </div>
        <div>
          <label for="password">Password:</label>
          <input type="password" v-model="password" id="password" required />
        </div>
        <button type="submit">Login</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        username: '',
        password: ''
      };
    },
    methods: {
      login() {
        // Simple login validation (replace with actual authentication)
        if (this.username === 'user' && this.password === 'password') {
          this.$router.push('/user-dashboard');
        } else {
          alert('Invalid credentials');
        }
      }
    }
  }
  </script>
  
  <style scoped>
  /* Add styles for the login form */
  </style>
  