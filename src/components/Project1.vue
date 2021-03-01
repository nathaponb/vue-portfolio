<template>
  <div class="one card">
      <router-link to="/about">
        <img src="../assets/todo-bg.jpg" alt="todo">
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