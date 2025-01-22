<template>
    <menu>
      <NavMenu class="desktop" />
      <MenuMobile class="show_in_mobile"> </MenuMobile>
      <!-- <button v-if="showMenuMobile" @click="showMenuMobile = false">close</button> -->
    </menu>
  </template>
  
  <script>
  import NavMenu from "./NavMenu.vue";
  import MenuMobile from "./MenuMobile.vue";
  export default {
    components: { NavMenu, MenuMobile },
    data() {
      return {};
    },
  };
  </script>
  
  <style lang="scss" scoped>
  menu {
    background: transparent;
    padding: 16px;
  
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 16px;
    border-radius: 16px;
    z-index: 100;
    transition: 800ms;
  
    .show_in_mobile {
      cursor: pointer;
      display: none;
    }
  
    @media (max-width: 1024px) {
      padding: 12px 24px;
      .show_in_mobile {
        display: flex;
      }
      .desktop {
        display: none;
      }
    }
  }
  
  .open-menu {
    display: none !important;
  }
  </style>
  