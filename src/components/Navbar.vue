<template>
    <nav class="topnav">
      <router-link class="active" to="/">Home</router-link>
      <router-link to="/tutorials" class="active">Tutorials</router-link>
      <router-link to="/about" class="active">About</router-link>
      <router-link to="/Form" class="active">Form</router-link>
    </nav>
  </template>


  <script>
  export default {
  
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  .topnav {
    background-color:black;
    overflow: hidden;
  }

  .active:hover {
    width: 100px;
    background-color: blueviolet;
  }

  router-link {
     width: 100px;
      float: left;
      color: white;
      text-align: center;
      padding: 14px 16px;
      text-decoration: none;
      font-size: 17px;
  }
  
  </style>