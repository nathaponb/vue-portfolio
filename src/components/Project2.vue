<template>
  <div class="two card">
    <a href="https://github.com/hellonathapon/react-ecommerce-app">
      <div class="overlay"></div>
      <img
        src="../assets/optimized-images/e-commerce.png"
        alt="e-commerce app"
      />
    </a>

    <article>
      <h2 class="en">E-Commerce App</h2>
      <p class="en">
        A feature rich and elegent Material Design online shopping project
      </p>
      <ul>
        <li>
          <a href="https://reactjs.org/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/react-2.svg" alt="react" />
          </a>
        </li>
        <li>
          <a href="https://redux.js.org/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/redux.svg" alt="redux" />
          </a>
        </li>
        <li>
          <a href="https://material-ui.com/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/md.svg" alt="material ui" />
          </a>
        </li>
      </ul>
    </article>

    <div class="choice">
      <a
        href="https://github.com/hellonathapon/react-ecommerce-app"
        target="_blank"
        ref="noreferrer"
        ><h2 class="en">Source code</h2></a
      >
      <a
        href="https://hellonathapon.github.io/react-ecommerce-app/#/"
        target="_blank"
        ref="noreferrer"
        ><h2 class="en">Live</h2></a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "Project2",
};
</script>

<style scoped lang="scss">
.two {
  grid-column: 1 / span 12;
  grid-row: 5 / 7;
  // For card, apply global style from home.vue
}

@media only screen and (min-width: 700px) {
  .two {
    grid-column: 9 / span 12;
    grid-row: 3 / 5;
  }
}
</style>
