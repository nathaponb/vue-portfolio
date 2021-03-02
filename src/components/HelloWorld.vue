<template>
  <div class="hello">
    <router-link to="/about">
      <img src="../assets/optimized-bg-hello.jpg" alt="hello">
    </router-link>

    <article>
      <h2>Hello World</h2>
      <p>My name is Nathapon Boontaungkaew</p>
      <p>A 25 years old Full-stack Webdeveloper (Javascript),</p>
      <p>Data Analyst (Python)</p>

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
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: calc(100% - 100px);
    /* background:crimson; */
    & > * {
      color: #fff;
    }
  }
}
</style>
