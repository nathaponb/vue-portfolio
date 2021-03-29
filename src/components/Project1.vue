<template>
  <div class="one card">
      <router-link to="/about">
      <div class="overlay"></div>
        <img src="../assets/news-app.png" alt="news-app-bg">
      </router-link>

      <article>
        <h2>News App</h2>
        <p>RestApi project</p>
        <ul>
            <li><a href="https://www.typescriptlang.org/" target="_blank" ref="noreferrer">
              <img src="../assets/svg/ts.svg" alt="typescript">
            </a></li>
            <li><a href="https://reactjs.org/" target="_blank" ref="noreferrer">
              <img src="../assets/svg/react-2.svg" alt="react">
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
    name: "Project1"
}
</script>

<style scoped lang="scss">
.one{
    grid-column: 1 / span 12;
    grid-row: 3 / 5;
    // For card, apply global style from home.vue 
}

@media only screen and (min-width: 700px) {
    .one{
        grid-column: 1 / span 8;
    }
}
</style>