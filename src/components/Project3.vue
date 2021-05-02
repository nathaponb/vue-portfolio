<template>
  <div class="three card">
    <a href="https://github.com/hellonathapon/oauth-google">
      <div class="overlay"></div>
      <img src="../assets/optimized-images/oauth.png" alt="oauth project" />
    </a>

    <article>
      <h2>OAuth Project</h2>
      <p>An secure Authorization in simple and standard</p>
      <ul>
        <li>
          <a href="https://getbootstrap.com/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/bootstrap.svg" alt="bootstrap" />
          </a>
        </li>
        <li>
          <a href="https://expressjs.com/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/express-1.svg" alt="express" />
          </a>
        </li>
        <li>
          <a href="http://www.passportjs.org/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/passport.svg" alt="passport" />
          </a>
        </li>
        <li>
          <a href="https://www.mongodb.com/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/mongodb-icon-1.svg" alt="mongodb" />
          </a>
        </li>
      </ul>
    </article>

    <div class="choice">
      <a
        href="https://github.com/hellonathapon/oauth-google"
        target="_blank"
        ref="noreferrer"
        ><h2>Source code</h2></a
      >
      <a
        href="https://oauth-google-cat.herokuapp.com/"
        target="_blank"
        ref="noreferrer"
        ><h2>Live</h2></a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "Project3",
};
</script>

<style scoped lang="scss">
.three {
  grid-column: 1 / span 12;
  grid-row: 7 / 9;
  // For card, apply global style from home.vue
}

@media only screen and (min-width: 700px) {
  .three {
    grid-column: 1 / span 6;
    grid-row: 5 / 7;
  }
}
</style>
