<template>
  <div class="header">
    <div id="nav">
      <div class="logo">
        <router-link to="/">
          <img
            src="../assets/optimized-images/profile_placeholder.png"
            alt="le me"
          />
        </router-link>
      </div>
      <article>
        <p class="name">Nathapon</p>
        <p class="sub-name">@hellonathapon</p>
        <!-- <div class="info">
          <div class="icon-info">
            <img src="../assets/svg/calendar.svg" alt="date icon" />
          </div>
          Born 8 June 1996
        </div> -->
        <div class="social-nav-icons">
          <a
            href="mailto:hellonathapon@gmail.com"
            target="_blank"
            ref="noreferrer"
            class="link email-icon"
            ><img src="../assets/svg/email.svg" alt="email icon"
          /></a>

          <a
            class="link github-icon"
            href="https://github.com/hellonathapon?tab=repositories"
            target="_blank"
            ref="noreferrer"
            ><img src="../assets/svg/github-2.svg" alt="github"
          /></a>

          <a
            href="https://www.facebook.com/natha.pon.56/"
            target="_blank"
            ref="noreferrer"
            class="link facebook-icon"
            ><img src="../assets/svg/Instagram-Icon-01.svg" alt="instagram icon"
          /></a>
        </div>
      </article>
      <section>
        <router-link class="link about-me-link" to="/about"
          >About Me</router-link
        >
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
$pri-col: #2c3e50;
$sec-col: rgb(91, 112, 131);

.header {
  grid-column: 1 / span 12;
  #nav {
    display: flex;
    flex-flow: row wrap;
    align-items: center;
    justify-content: space-between;
    padding: 0.5rem 1rem;
    box-shadow: 0 1px 3px 0 rgb(0 0 0 / 10%), 0 1px 2px 0 rgb(0 0 0 / 6%);
    /* background: pink; */

    .logo {
      width: 50px;
      height: 50px;
      overflow: hidden;
      border-radius: 50%;

      a {
        img {
          width: 100%;
        }
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
    article {
      display: none;
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
          width: 70px;
          height: 70px;
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
    width: 300px;
    position: fixed;

    #nav {
      flex-direction: column;
      justify-content: flex-start;
      align-items: flex-start;
      height: 100vh;
      box-shadow: none;
      /* width: 100%; */
      /* background: pink; */

      .logo {
        width: 150px;
        height: 150px;
        overflow: hidden;
        /* border: 2px solid #2c3e50; */
        img {
          width: 100%;
        }
      }
      .about-me-link {
        display: block;
        font-size: 2rem;
        margin: 0.5rem 0;
        font-weight: 200;
      }

      article {
        display: block;
        text-align: center;
        width: 150px;
        .name {
          font-weight: 700;
        }
        .sub-name {
          color: $sec-col;
        }
        .info {
          margin-top: 0.5rem;
          display: flex;
          .icon-info {
            width: 20px;
            height: 20px;
            overflow: hidden;
            /* margin-right: 0px; */
          }
        }
        .social-nav-icons {
          display: flex;
          justify-content: space-around;
          align-items: center;
          margin-top: 0.5rem;
          .link {
            width: 30px;
            height: 30px;
            img {
              width: 100%;
            }
          }
          /* .link:not(:last-child) {
            margin-right: 0.5rem;
          } */
        }
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
