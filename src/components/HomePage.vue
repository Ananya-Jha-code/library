<template>
    <div class="home">
      <h1>Library Management System</h1>
      <button @click="navigateTo('librarian-login')">Librarian Login</button>
      <button @click="navigateTo('user-login')">User Login</button>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      navigateTo(route) {
        this.$router.push(`/${route}`);
      }
    }
  }
  </script>
  
  <style scoped>
  button {
    margin: 10px;
    padding: 10px;
    font-size: 16px;
  }
  </style>