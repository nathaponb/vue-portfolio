<template>
  <div class="three card">
      <router-link to="/about">
        <img src="../assets/tank-bg.jpg" alt="chart">
      </router-link>

      <article>
        <h2>Hello There</h2>
        <ul>
            <li><a href="https://www.google.com/" target="_blank">Google</a></li>
        </ul>
      </article>
  </div>
</template>

<script>
export default {
    name: "Project3"
}
</script>

<style scoped lang="scss">
.three{
    grid-column: 1 / span 12;
    grid-row: 5 / 8;
    // For card, apply global style from home.vue 
}

@media only screen and (min-width: 700px) {
    .three{
        grid-column: 1 / span 12;
    }
}

</style>