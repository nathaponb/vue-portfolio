<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<script>
export default {
  name: "About"
}
</script>

<style scoped lang="scss">
/**
 * Direct Grid child of App.vue component
 */
.about {
    grid-column: 1 / span 12;
  }

  @media only screen and (min-width: 700px) {
    .about {
      grid-column: 3 / span 12;
    }
  }
</style>
