<template>
    <div class="footer">
        <h3>Footer</h3>
        <p class="footer-text-centre">
        <routerlink class="menu" to="/">Home</routerlink>
        <routerlink to="/" class="menu">Tutorials</routerlink>
        <routerlink to="/" class="menu">About</routerlink>
        </p>
     
    </div>
  </template>


  <script>
  export default {
  
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
 
  .footer{
        position: relative;
        bottom:0;
        left: 0;
        width: 100%;
        height: 100px;
        background-color: black;
        color: white;
  
  }
  .footer-text-left{
    font-size: 25px;
   padding-left: 40px;
    float: left;
    word-spacing: 50px;
  }
  .menu:hover{
    background-color: blueviolet;
    font-size: 20px;
    padding: 14px 16px;
  }
  </style>