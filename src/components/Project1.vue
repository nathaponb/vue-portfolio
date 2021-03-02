<template>
  <div class="one card">
      <router-link to="/about">
      <div class="overlay"></div>
        <img src="../assets/todo-bg.jpg" alt="todo">
      </router-link>

      <article>
        <h2>Vue Todo App</h2>
        <ul>
            <li><a href="https://www.python.org/" target="_blank">
              <img src="../assets/svg/python-5.svg" alt="python">
            </a></li>
            <li><a href="https://www.python.org/" target="_blank">
              <img src="../assets/svg/md.svg" alt="md">
            </a></li>
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