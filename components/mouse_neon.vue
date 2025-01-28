<template>
    <div class="neon-cursor" :style="cursorStyle"></div>
  </template>
  
  <script setup>
  import { ref, onMounted, onBeforeUnmount } from 'vue'
  
  const cursorX = ref(0)
  const cursorY = ref(0)
  
  const cursorStyle = ref({})
  
  onMounted(() => {
    const updateCursor = (event) => {
      cursorX.value = event.clientX
      cursorY.value = event.clientY
  
      cursorStyle.value = {
        left: `${cursorX.value}px`,
        top: `${cursorY.value}px`,
      }
    }
  
    window.addEventListener('mousemove', updateCursor)
  })
  
  onBeforeUnmount(() => {
    window.removeEventListener('mousemove', updateCursor)
  })
  </script>
  
  <style scoped>
  .neon-cursor {
    position: fixed;
    width: 360px;
    height: 360px;
    background: radial-gradient(circle, rgb(1, 135, 14) 0%, rgba(12, 254, 77, 0.6) 70%);
    border-radius: 50%;
    pointer-events: none;
    transform: translate(-50%, -50%);
    /*box-shadow: 0 0 20px rgba(0, 220, 22), 0 0 40px rgba(4, 247, 69, 0.6);*/
    transition: transform 0.1s ease, background-color 0.2s ease;
    filter: blur(100px);
  }
  </style>
  