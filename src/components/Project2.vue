<template>
  <div class="two card">
      <router-link to="/about">
        <img src="../assets/chart-bg.jpg" alt="chart">
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
    name: "Project2"
}
</script>

<style scoped lang="scss">
.two{
    grid-column: 1 / span 12;
    grid-row: 2 / 3;
    // For card, apply global style from home.vue 
}

@media only screen and (min-width: 700px) {
    .two{
        grid-column: 9 / span 12;
        grid-row: 3 / 5;
    }
}

</style>