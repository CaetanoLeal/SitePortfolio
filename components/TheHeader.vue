<template>
    <header class="header">
      <div class="container">
        <div class="content">
          <img
          />
          <MenuBar />
        </div>
      </div>
    </header>
  </template>
  
  <script>
  import MenuBar from "./MenuBar.vue";
  export default { components: { MenuBar } };
  </script>
  
  <style lang="scss" scoped>
  .header {
    height: 60px;
    background: rgb(0, 0, 0);
  }
  .container {
    backdrop-filter: blur(10px);
  
    width: 100%;
    height: 80px;
    background: #0000007f;
    position: fixed;
    z-index: 200;
    border-bottom: 2px solid rgb(1, 204, 1);
    box-shadow: 0px 6px 10px rgba(44, 243, 4, 0.5);
    /* position: absolute; */
  
    .content {
      display: flex;
      height: 100%;
      justify-content: space-between;
      align-items: center;
    }
  }
  </style>
  