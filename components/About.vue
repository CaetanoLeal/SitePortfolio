<!--<template>
    <section>

    </section>
</template>

<style scooped>
table {
    border: solid 2px;
    border-color: rgb(1, 204, 1);
    box-shadow: rgb(0, 120, 14) 2px 7px 14px;
}
td{
    border-right: solid 2px;
    border-color: rgb(1, 204, 1);
    box-shadow: rgb(0, 120, 14) 2px 7px 14px;
}

</style>-->

<template>
    <main class="container" id="magnificat">
      <div class="content" data-aos="fade-in">
        <img
          src="../assets/images/mao-no-queixo2.png"
          alt="icone da leal"
          width="300"
          data-aos="fade-up"
          data-aos-duration="800"
          data-aos-delay="300"
        />
        <div align="center">
        <table>
        <tr>
            <td>
            <h2>Front-end ⭐⭐⭐</h2>
            <p>
                <img src="https://www.vectorlogo.zone/logos/nuxtjs/nuxtjs-icon.svg" alt="nuxtjs" width="60" height="60"/>
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original-wordmark.svg" alt="vuejs" width="60" height="60"/>
                <img src="https://bestofjs.org/logos/vuetify.svg" alt="vuetify" width="60" height="60"/>
            </p>
            </td>
            <td>
            <h2>Database ⭐⭐⭐</h2>
            <p>
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="60" height="60"/>
                <img src="https://www.vectorlogo.zone/logos/sqlite/sqlite-icon.svg" alt="sqlite" width="60" height="60"/>
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="60" height="60"/>
            </p>
            </td>
            <td>
            <h2>Mobile ⭐⭐</h2>
            <p>
                <img src="https://www.vectorlogo.zone/logos/dartlang/dartlang-icon.svg" alt="dart" width="60" height="60"/>
                <img src="https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg" alt="flutter" width="60" height="60"/>
            </p>
            </td>
            <td>
            <h2>Back-end ⭐</h2>
            <p>
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="60" height="60"/>
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="60" height="60"/>
            </p>
            </td>
        </tr>
        </table>
    </div>
        <article data-aos="fade-up" data-aos-duration="800" data-aos-delay="600">
          <h2 class="gold">A Magnifica</h2>
          <h1 class="gold">Venha conhecer nossa distribuidora</h1>
          <p>
            Distribuidora especializada em temperos e variedades. Oferencendo
            desde sempre os melhores preços do estado
          </p>
          <p>
            Há mais 2 anos fornecendo os produtos com as melhores qualidades e
            variedade.
          </p>
          <p>
            Proporcionado aos nossos clientes prosperidade e alegria com cada um
            de nossos produtos.
          </p>
          <nuxt-link to="leal">
            <TheButton :title="'Conhecer mais'" class="golden_black_button" />
          </nuxt-link>
        </article>
      </div>
    </main>
  </template>
  
  <script>
  import TheButton from "./TheButton.vue";
  export default { components: { TheButton } };
  </script>
  
  <style lang="scss" scoped>
  .container {
    .content {
      min-height: 100vh;
      padding: 48px 16px;
      display: flex;
      justify-content: space-evenly;
      align-items: center;
  
      @media (max-width: 1024px) {
        flex-direction: column;
        img {
          width: 100px;
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
  
      .golden_black_button {
        background-color: black;
        color: gold;
      }
  
      .golden_black_button:hover {
        background-color: gold;
        color: black;
      }
    }
  }
  
  .container {
    height: calc(100vh);
  
    background-image: url("../assets/images/wallpaper_sessao_1.png");
    background-size: cover;
  }
  
  .gold {
    background: linear-gradient(
      90deg,
      rgba(207, 210, 69, 1) 0%,
      rgba(251, 251, 150, 1) 43%,
      rgba(233, 237, 53, 1) 98%
    );
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    color: var(--blue-300);
  }
  
  p {
    color: white;
  }
  table {
    border: solid 2px;
    border-color: rgb(1, 204, 1);
    box-shadow: rgb(0, 120, 14) 2px 7px 14px;
}
td{
    border-right: solid 2px;
    border-color: rgb(1, 204, 1);
    box-shadow: rgb(0, 120, 14) 2px 7px 14px;
}
  </style>
  