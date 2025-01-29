<template>
    <main class="container" id="about">
      <div class="content" data-aos="fade-in">
        <img
          src="../assets/images/mão_no_queixo.png"
          alt="mao_no_queixo"
          data-aos="fade-up"
          data-aos-duration="800"
          data-aos-delay="300"
        />
        <article data-aos="fade-up" data-aos-duration="800" data-aos-delay="600">
          <h1>I am {your role here}</h1>
          <p>
            your professional objective Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
          </p>
          <p>
            I have X years of experience in the technology field and have worked in:<br>
            <img class="icon" src="../assets/images/logo-leal.png" />
              Company name, yy/mm/dd - present day<br>
            <img class="icon" src="../assets/images/magalhaes-logo.jpg" />
              Company name, yy/mm/dd - yy/mm/dd<br>
            <img class="icon" src="../assets/images/rk-logo.png" />
              Company name, yy/mm/dd - yy/mm/dd<br>
          </p>
          <p>
            i speak english, {your native language} and {others languages can you speak}
          </p>
            <TheButton :title="'SEE MY PROJECTS'" />
        </article>
      </div>
    </main>
  </template>
  
  <script lang="ts">
  import TheButton from "./TheButton.vue";
  
  export default defineComponent({
    components: {
      TheButton,
    },
  });
  </script>
  
  <style lang="scss" scoped>
  .container {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 90vh;
  }
  
  .content {
    max-height: 100vh; 
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 180px;
  
    @media (max-width: 1024px) {
      flex-direction: column;
      img {
        width: 100px;
        height: auto;
      }
      article {
        text-align: center;
      }
    }
  
    article {
      margin-top: 24px;
      max-width: 600px;
  
      h1 {
        font-size: 2.5rem;
      }
      h1,
      h2 {
        color: var(--blue-300);
      }
      p {
        margin-bottom: 2rem;
      }
    }
  }
  
  img {
    height: 90vh;
    width: auto;
    max-width: 100%;
  }
  
  p {
    color: white;
  }
  
  .icon {
    width: 40px;
    height: 40px;
  }
  </style>