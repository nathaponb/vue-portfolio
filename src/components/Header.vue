<template>
  <div class="header">
    <div id="nav">
      <div class="logo">
        <router-link to="/">
          <img src="../assets/profile-pic.jpg" alt="logo" />
        </router-link>
      </div>
      <router-link class="link" to="/about">About Me</router-link>
      <a
        class="link"
        href="https://github.com/hellonathapon?tab=repositories"
        target="_blank"
        ref="noreferrer"
        >Github</a
      >
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
    flex-flow: column wrap;
    align-items: flex-start;
    padding: 0.5rem 1rem;

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
    .link {
      display: none;
    }
  }
}

@media only screen and (min-width: 700px) {
  .header {
    grid-column: 1 / span 3;

    #nav {
      position: sticky;
      top: 0;

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
    }
  }
}
</style>
