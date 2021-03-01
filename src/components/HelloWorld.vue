<template>
  <div class="hello">
    <router-link to="/about">
      <img src="../assets/optimized-bg-hello.jpg" alt="hello">
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
  name: 'HelloWorld',
}
</script>

<style scoped lang="scss">
/**
 * direct grid child of Home 
 */
.hello{
  grid-column: 1 / span 12;
  grid-row: 1 / span 2;
  position: relative;
  
  a{
    overflow: hidden;
    img{
      object-fit: cover;
      object-position: center;
      height: 100%;
      width: 100%;
    }
  }

  article{
    position: absolute;
    top: 0;
    right: 0;
  }
}
</style>
