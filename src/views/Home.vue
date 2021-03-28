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
  grid-template-rows: repeat(6, 12rem);

  /**
   * Global style for chridren
   */
  .card{
    position: relative;
    overflow: hidden;

    /* display choices */
    &:hover > .choice{
      opacity: 1;
      pointer-events: auto;
    }
  
    a{
      overflow: hidden;
      &:hover img{
        transform: scale(1.1);
      }
      .overlay{
        z-index: 10;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.3);
        transition: all 0.3s ease;
      }
      img{
        object-fit: cover;
        object-position: center;
        height: 100%;
        width: 100%;
        transition: all .3s ease;
      }
    }

    article{
      z-index: 20;
      position: absolute;
      top: 0;
      right: 0;
      h2{
        color: #fff;
      }
      ul{
        li{
          display: inline-block;
          padding: .5rem;
          list-style: none;
          transition: all .1s ease;
          &:hover{
            transform: scale(1.01);
          }
          a{
            text-decoration: none;
            img{
              width: 50px;
            }
          }
        }
      }
    }

    .choice {
      z-index: 20;
      position: absolute;
      top: 50%;
      left: 50%;
      color: #fff;
      transform: translate(-50%, -50%);
      transition: all .3s ease-in-out;
      opacity: 0;
      pointer-events: none;
      a {
        text-decoration: none;
        color: #fff;
      }
    }
  }
}

@media only screen and (min-width: 700px) {
  .home {
    grid-column: 4 / span 12;
  }
}
</style>
