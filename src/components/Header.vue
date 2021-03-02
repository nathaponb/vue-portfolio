<template>
  <div class="header">
      <div id="nav">
          <div class="logo">
              <router-link to="/">
                  <img src="../assets/kermit.png" alt="logo">
              </router-link>
          </div>
          <router-link class="link" to="/about">About</router-link>
          <a class="link" href="https://github.com/hellonathapon?tab=repositories" target="_blank">Github</a>
      </div>
  </div>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped lang="scss">
.header {
    grid-column: 1 / span 12;
    #nav {
        display: flex;
        flex-flow: column wrap;
        align-items: flex-start;
        padding: 0.5rem 1rem;

        .logo{
            img{
                width: 40px;
            }
        }
        a {
            font-weight: bold;
            color: #2c3e50;
            text-decoration: none;

            &.router-link-exact-active {
            color: #42b983;
            }
        }
        .link{
            display: none;
        }
    }
}

@media only screen and (min-width: 700px) {
    .header {
        grid-column: 1 / span 3;

        #nav{
            position: sticky;
            top: 0;
            
            .logo{
                img{
                    width: 100px;
                }
            }
            .link{
                display: block;
                font-size: 2rem;
                margin: .5rem 0;
                font-weight: 200;
            }
        }
    }
}
</style>