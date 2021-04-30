<template>
  <div class="header">
    <div id="nav">
      <div class="logo">
        <router-link to="/">
          <img src="../assets/profile-pic.jpg" alt="logo" />
        </router-link>
      </div>
      <section>
        <router-link class="link about-me-link" to="/about"
          >About Me</router-link
        >
        <div>
          <a
            class="link github-icon"
            href="https://github.com/hellonathapon?tab=repositories"
            target="_blank"
            ref="noreferrer"
            ><img src="../assets/svg/github.svg" alt="github"
          /></a>

          <a
            href="https://www.facebook.com/natha.pon.56/"
            target="_blank"
            ref="noreferrer"
            class="link facebook-icon"
            ><img src="../assets/svg/facebook.svg" alt="facebook icon"
          /></a>
        </div>
      </section>
      <div class="coppyright">@open source, {{ new Date().getFullYear() }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped lang="scss">
.header {
  grid-column: 1 / span 12;
  #nav {
    display: flex;
    flex-flow: row wrap;
    align-items: center;
    justify-content: space-between;
    padding: 0.5rem 1rem;
    box-shadow: 0 1px 3px 0 rgb(0 0 0 / 10%), 0 1px 2px 0 rgb(0 0 0 / 6%);

    .logo {
      width: 50px;
      height: 50px;
      overflow: hidden;
      border-radius: 50%;
      img {
        width: 100%;
      }
    }
    a {
      font-weight: bold;
      color: #2c3e50;
      text-decoration: none;

      &.router-link-exact-active {
        color: #42b983;
      }
    }
    section {
      display: flex;
      .about-me-link {
        margin-right: 1rem;
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
      }
      div {
        display: flex;
        align-items: center;
        .github-icon {
          width: 50px;
          height: 50px;
        }
        .facebook-icon {
          width: 43px;
          height: 43px;
          margin-left: 0.7rem;
        }
      }
    }
    .coppyright {
      display: none;
    }
  }
}

@media only screen and (min-width: 700px) {
  .header {
    grid-column: 1 / span 3;

    #nav {
      position: fixed;
      top: 0;
      flex-direction: column;
      justify-content: flex-start;
      align-items: flex-start;
      height: 100vh;
      box-shadow: none;
      /* width: 100%; */

      .logo {
        width: 150px;
        height: 150px;
        overflow: hidden;
        /* border: 2px solid #2c3e50; */
        img {
          width: 100%;
        }
      }
      .link {
        display: block;
        font-size: 2rem;
        margin: 0.5rem 0;
        font-weight: 200;
      }
      section {
        flex-direction: column;
        div {
          display: flex;
          justify-content: flex-start;
          align-items: center;
          .facebook-icon {
            margin-left: 0.5rem;
          }
        }
      }
      .coppyright {
        display: block;
        position: absolute;
        bottom: 1rem;
        left: 1rem;
      }
    }
  }
}
</style>
