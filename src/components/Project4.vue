<template>
  <div class="todo-app card">
    <a href="https://github.com/hellonathapon/todo-app">
      <div class="overlay"></div>
      <img src="../assets/todo-app-thumbnail.png" alt="todo app project" />
    </a>

    <article>
      <h2>Todo App Project</h2>
      <p>Simple elegant authorize user via popular platforms</p>
      <ul>
        <li>
          <a href="https://v3.vuejs.org/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/vue-js-1.svg" alt="vuejs" />
          </a>
        </li>
        <li>
          <a href="https://expressjs.com/" target="_blank" ref="noreferrer">
            <img src="../assets/svg/express-1.svg" alt="expressjs" />
          </a>
        </li>
        <li>
          <a
            href="https://github.com/mysqljs/mysql"
            target="_blank"
            ref="noreferrer"
          >
            <img src="../assets/svg/mysql-7.svg" alt="mysql" />
          </a>
        </li>
      </ul>
    </article>

    <div class="choice">
      <a
        href="https://github.com/hellonathapon/todo-app"
        target="_blank"
        ref="noreferrer"
        ><h2>Source code</h2></a
      >
      <a
        href="https://infinite-oasis-31102.herokuapp.com/"
        target="_blank"
        ref="noreferrer"
        ><h2>Live</h2></a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "Project4",
};
</script>

<style scoped lang="scss">
.todo-app {
  grid-column: 1 / span 12;
  grid-row: 9 / 11;
  // For card, apply global style from home.vue
}

@media only screen and (min-width: 700px) {
  .todo-app {
    grid-column: 7 / span 12;
    grid-row: 5 / 7;
  }
}
</style>
