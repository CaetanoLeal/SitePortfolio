<template>
    <nav class="navbar">
      <a href="#hero">HERO</a>
      <a href="#about">ABOUT</a>
      <a href="#portfolio">PORTFOLIO</a>
      <a href="#porque">CONTACT</a>
    </nav>
  </template>
  
  <script>
  export default {};
  </script>
  
  <style lang="scss" scoped>
  .navbar {
    display: flex;
    gap: 40px;
    a {
      color: white;
      font-family: 'Retropix';
      font-size: 20px;
      &:hover {
        color: rgb(1, 204, 1);
      }
    }
    @media (max-width: 1024px) {
      padding: 12px 24px;
    }
  }
  </style>
  