<template>
  <div class="one card">
    <a href="https://github.com/hellonathapon/react-ts-news-app">
      <div class="overlay"></div>
      <img
        src="../assets/optimized-images/news-app-thumbnail.png"
        alt="news-app-bg"
      />
    </a>

    <article>
      <h2 class="en">React News App</h2>
      <p class="en">
        A simple React App to keep you updated with latest global news.
      </p>
      <ul>
        <li>
          <a
            href="https://www.typescriptlang.org/"
            target="_blank"
            ref="noreferrer"
          >
            <img src="../assets/svg/ts.svg" alt="typescript" />
          </a>
        </li>
        <li>
          <a href="https://reactjs.org/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/react-2.svg" alt="react" />
          </a>
        </li>
      </ul>
    </article>

    <div class="choice">
      <a
        href="https://github.com/hellonathapon/react-ts-news-app"
        target="_blank"
        ref="noreferrer"
        ><h2 class="en">Source code</h2></a
      >
      <a
        href="https://react-ts-news-app.herokuapp.com/"
        target="_blank"
        ref="noreferrer"
        ><h2 class="en">Live</h2></a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "Project1",
};
</script>

<style scoped lang="scss">
.one {
  grid-column: 1 / span 12;
  grid-row: 3 / 5;
  // For card, apply global style from home.vue
}

@media only screen and (min-width: 700px) {
  .one {
    grid-column: 1 / span 8;
    grid-row: 3 / 5;
  }
}
</style>
