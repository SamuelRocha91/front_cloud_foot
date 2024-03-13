<script setup lang="ts">
import { RouterLink } from 'vue-router';
</script>

<template>
  <header>
    <nav class="links-about">
      <a href="#about">Sobre</a>
      <a href="#rule">Funcionamento</a>
      <a href="#id">Dúvidas</a>
    </nav>
    <nav class="links-login">
      <img src="../../public/logo01.png" alt="Nuvem em chamas" />
      <RouterLink class="routes-header" to="/registro">Registro</RouterLink>
      <RouterLink class="routes-header" to="/login">Login</RouterLink>
    </nav>
  </header>
</template>

<style scoped>
  header {
    background-color: rgb(0, 0, 0);
    color: white;
    display: flex;
    height: 10vh;
    font-size: 25px;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    text-decoration: none;
  }
 .links-login {
  display: flex;
  width: 50%;
  align-items: center;
  align-content: center;
  gap: 30px;
  justify-content: end;
  margin: 0 100px 0 0;
 }

 .links-login a {
  text-decoration: none;
  color: #ffffff;
 }
  .links-about {
  display: flex;
  width: 50%;
  align-items: center;
  gap: 50px;
  justify-content: start;
  margin: 0 0 0 100px;
 }

 .links-about a{
   text-decoration: none;
   color: #ffffff;
 }

 @media (max-width: 1260px) {
   .links-about {
    gap: 30px;
    margin: 0 0 0 60px;
    text-decoration: none;

   }

    .links-login {
      gap: 20px;
      margin: 0 60px 0 0;
      text-decoration: none;

   }
  }
  @media (max-width: 1000px) {
   .links-about {
    gap: 20px;
    margin: 0 0 0 40px;
    text-decoration: none;

   }

    .links-login {
      gap: 15px;
      margin: 0 40px 0 0;
      text-decoration: none;

   }
  }
   @media (max-width: 420px) {
   .links-about {
    display: none;

   }
    .links-login {
      gap: 35px;
      width: 100%;
      margin: 0 40px 0 0;
      display: flex;
      justify-content: end;
      text-decoration: none;

   }
   .links-login img {
     display: none;
      
   }
  }

   @media (max-width: 360px) {
   .links-about {
    display: none;

   }
    .links-login {
      gap: 15px;
      width: 100%;
      margin: 0 40px 0 0;
      display: flex;
      justify-content: start;
      text-decoration: none;

   }
   .links-login img {
      width: 100%;
      margin: 0 40px 0 0;
   }
  }
  @media (max-width: 760px) {
   .links-about {
    display: none;
   }
    .links-login {
      gap: 35px;
      width: 100%;
      display: flex;
      justify-content: center;
      text-decoration: none;
   }

  }
</style>