<template>
    <div>
      <div class="form-container">
        <h2>Login</h2>
        <form @submit.prevent="login">
          <label for="loginUsername">Username:</label>
          <input type="text" id="loginUsername" v-model="loginUsername" required>
          <label for="loginPassword">Password:</label>
          <input type="password" id="loginPassword" v-model="loginPassword" required>
          <button type="submit">Login</button>
        </form>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        loginUsername: '',
        loginPassword: ''
      };
    },
    
  };
  </script>
  
  <style scoped>
  body {
    font-family: Arial, sans-serif;
    background-color: #65faf2;
  }
  
  .form-container {
    background-color: #030a3a;
    border: 1px solid #10a1ef;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    max-width: 300px;
    margin: 0 auto;
  }
  
  h2 {
    text-align: center;
    color: antiquewhite;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
    color: antiquewhite;
  }
  
  input[type="text"],
  input[type="password"] {
    width: 100%;
    padding: 8px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
  }
  
  button[type="submit"] {
    background-color: #007bff;
    color: #fff;
    border: none;
    padding: 10px 20px;
    border-radius: 3px;
    cursor: pointer;
  }
  
  button[type="submit"]:hover {
    background-color: #0056b3;
  }
  </style>
  