<template>
  <div class="three card">
      <router-link to="/about">
        <div class="overlay"></div>
        <img src="../assets/tank-bg.jpg" alt="chart">
      </router-link>

      <article>
        <h2>Hello There</h2>
        <ul>
            <li><a href="https://www.google.com/" target="_blank">
              <img src="../assets/svg/react-2.svg" alt="react">
            </a></li>
            <li><a href="https://www.python.org/" target="_blank">
              <img src="../assets/svg/python-5.svg" alt="python">
            </a></li>
        </ul>
      </article>

      <div class="choice">
        <a href="https://reactjs.org/" target="_blank" ref="noreferrer"><h2>Source code</h2></a>
        <a href="https://reactjs.org/" target="_blank" ref="noreferrer"><h2>Live</h2></a>
      </div>
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
    grid-row: 5 / 7;
    // For card, apply global style from home.vue 
}

@media only screen and (min-width: 700px) {
    .three{
        grid-column: 1 / span 12;
    }
}

</style>