<template>
  <div class="hero">
    <MouseNeon /> <!-- Efeito neon do mouse -->
    <div class="content-wrapper">
      <div class="content">
        <h1>welcome to my website</h1>
        <p>i am full stack developer</p>
      </div>
      <img
        src="../assets/images/bracos-cruzados.png"
        width="400"
        data-aos="fade-up"
        data-aos-duration="800"
        data-aos-delay="300"
        class="hero-image"
      />
    </div>
  </div>
</template>

<script setup>
import MouseNeon from './mouse_neon.vue'; // Importe o componente
</script>

<style scoped>
.hero {
  position: relative; /* Necessário para que os elementos absolutos fiquem relativos a este contêiner */
  width: 100%;
  height: 99vh;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden; /* Garante que nada escape do contêiner */
  background: rgb(0, 97, 11);
  background: linear-gradient(0deg, rgba(0, 97, 11, 1) 0%, rgba(0, 0, 0, 1) 20%);
}

.content-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 90%; /* Ajuste conforme necessário */
  max-width: 1200px;
  position: relative; /* Não é estritamente necessário, mas pode ser útil para organizar o layout */
}

.content {
  color: white;
}

.hero-image {
  position: absolute; /* Torna o posicionamento relativo ao contêiner .hero */
  bottom: 0;          /* Alinha a imagem na parte inferior */
  right: 0;           /* Alinha a imagem à direita */
  width: 400px;       /* Define o tamanho da imagem */
  max-width: 50%;     /* Garante que a imagem não exceda 50% do contêiner */
}

h1 {
  font-size: 3rem;
}

p {
  font-size: 1.5rem;
}
</style>