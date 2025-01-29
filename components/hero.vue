<template>
  <div class="hero">
    <MouseNeon /> <!-- Efeito neon do mouse -->
    <div class="content-wrapper">
      <div class="content">
        <h1>YOUR NAME HERE</h1>
        <p>Loren ipsun dolor sit anet, consectetur adipisci elit, sed eiusnod tenpor incidunt ut labore et dolore nagna aliqua.</p>
        <TheButton :title="'Entrar em contato'" />
      </div>
      <img
        src="../assets/images/bracos-cruzados.png"
        data-aos="fade-up"
        data-aos-duration="800"
        data-aos-delay="300"
        class="hero-image"
      />
    </div>
  </div>
</template>

<script setup>
import MouseNeon from './mouse_neon.vue';
</script>

<style scoped>
.hero {
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  background: rgb(0, 97, 11);
  background: linear-gradient(0deg, rgba(0, 97, 11, 1) 0%, rgba(0, 0, 0, 1) 20%);
}

.content-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  position: relative;
}

.content {
  color: white;
  margin-right: 30vw;
}

.hero-image {
  position: absolute;
  height: 100vh;
  right: 0;
  width: initial;
}

h1 {
  font-size: 3rem;
}

p {
  font-size: 1.5rem;
}
</style>