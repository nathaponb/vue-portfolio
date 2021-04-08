<template>
  <div class="three card">
      <router-link to="/about">
        <div class="overlay"></div>
        <img src="../assets/oauth.png" alt="oauth project">
      </router-link>

      <article>
        <h2>OAuth Project</h2>
        <p>Simple elegant authorize user via popular platforms</p>
        <ul>
            <li><a href="https://www.google.com/" target="_blank" ref="noreferrer">
              <img src="../assets/svg/express-1.svg" alt="express">
            </a></li>
            <li><a href="https://www.google.com/" target="_blank" ref="noreferrer">
              <img src="../assets/svg/passport.svg" alt="passport">
            </a></li>
            <li><a href="https://www.google.com/" target="_blank" ref="noreferrer">
              <img src="../assets/svg/ejs.svg" alt="ejs">
            </a></li>
            <li><a href="https://www.python.org/" target="_blank" ref="noreferrer">
              <img src="../assets/svg/bootstrap.svg" alt="bootstrap">
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
        grid-column: 1 / span 6;
    }
}

</style>