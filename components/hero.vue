<template>
    <div class="hero">
      <MouseNeon /> <!-- Efeito neon do mouse -->
      <div class="content">
        <h1>Bem-vindo ao Hero Section</h1>
        <p>Adicione aqui o conteúdo do seu Hero</p>
      </div>
    </div>
  </template>
  
  <script setup>
  import MouseNeon from './mouse_neon.vue'; // Importe o componente
  </script>
  
  <style scoped>
  .hero {
    position: relative;
    width: 100%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden; /* Garante que nada escape do contêiner */
    background-color: #000; /* Fundo para destacar o efeito */
  }
  
  .content {
    position: relative; /* Garante que o texto fique acima do efeito */
    z-index: 1;
    text-align: center;
    color: white;
  }
  
  h1 {
    font-size: 3rem;
  }
  
  p {
    font-size: 1.5rem;
  }
  </style>
  