<template>
    <div class="pi">
      <img
        @click="showMenuMobile = !showMenuMobile"
        src="../assets/images/Menu.png"
        width="30px"
        class="show_in_mobile"
      />
      <menu class="menu__mobile" :class="{ open__menu: showMenuMobile }">
        <nav class="navbar">
          <a href="#inicio" @click="closeMenu">Inicio </a>
          <a href="#leal" @click="closeMenu">A Leal</a>
          <a href="#softwares" @click="closeMenu">Softwares</a>
          <a href="#porque" @click="closeMenu">Porque nos escolher</a>
          <a href="#onde" @click="closeMenu">Onde estamos</a>
          <a href="#proposta" @click="closeMenu">Solicitar proposta</a>
        </nav>
      </menu>
    </div>
  </template>
  
  <script>
  import NavMenu from "./NavMenu.vue";
  export default {
    components: { NavMenu },
    props: {},
    data() {
      return {
        showMenuMobile: false,
      };
    },
    methods: {
      closeMenu() {
        setTimeout(() => {
          this.showMenuMobile = false;
        }, 400);
      },
    },
  };
  </script>
  
  <style lang="scss" scoped>
  .open__menu {
    right: 0 !important;
    opacity: 1 !important;
    width: 100vw !important;
  }
  
  .menu__mobile {
    z-index: 1000;
    padding: 10px;
    width: 100px;
    height: 100vh;
    border-radius: 0;
  
    justify-content: center;
    position: absolute;
    transition: 0.5s;
    opacity: 0;
    top: 80px;
    right: -300px;
    background: #111721ec !important;
    .navbar {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      a {
        text-align: center;
        padding: 16px;
        transition: 0.1s;
        margin-bottom: 4px;
        font-size: 1.2rem;
        color: var(--gray-200);
        &:hover {
          transform: scale(1.05);
          color: var(--white);
        }
      }
    }
  }
  </style>
  