<template>
  <div class="header">
      <div id="nav">
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link>
      </div>
  </div>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped lang="scss">
.header {
    grid-column: 1 / span 12;
    #nav {
    /* padding: 30px; */

    a {
        font-weight: bold;
        color: #2c3e50;

        &.router-link-exact-active {
        color: #42b983;
        }
    }
    }
}

@media only screen and (min-width: 700px) {
    .header {
        grid-column: 1 / span 3;
    }
}
</style>