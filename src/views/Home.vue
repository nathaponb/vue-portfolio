<template>
  <div class="home">
    <HelloWorld />
    <Project1 />
    <Project2 />
    <Project3 />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Project1 from '@/components/Project1.vue'
import Project2 from '@/components/Project2.vue'
import Project3 from '@/components/Project3.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Project1,
    Project2,
    Project3,
  }
}
</script>

<style lang="scss">
/**
 * Direct Grid child of App.vue component
 */
.home {
  grid-column: 1 / span 12;

  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(12, 12rem);

  /**
   * Global style for chridren
   */
  .card{
    position: relative;
    overflow: hidden;
  
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
}

@media only screen and (min-width: 700px) {
  .home {
    grid-column: 4 / span 12;
  }
}
</style>
