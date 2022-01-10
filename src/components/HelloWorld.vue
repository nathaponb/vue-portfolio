<template>
  <div class="hello">
    <article>
      <h1 class="name">Nathapon Boonthongkaew</h1>
      <p>
        Hello world! 👋 My name is "Nathapon Boonthongkaew", i am a full-stack
        web developer, i have a solid knowledge of Javascript and its
        ecosystems. I also have an intermediate Python skill for Data Analytics.
      </p>
    </article>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
};
</script>

<style scoped lang="scss">
/**
 * direct grid child of Home 
 */
.hello {
  grid-column: 1 / span 12;
  grid-row: 1 / span 2;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-family: Quicksand;
  /* background: linear-gradient(rgba(29, 38, 113, 0.6), rgba(195, 55, 100, 0.6)); */
  background-image: linear-gradient(
      to right,
      rgba(29, 38, 113, 0.6),
      rgba(195, 55, 100, 0.6)
    ),
    url("../assets//optimized-images/blake-connally-B3l0g6HLxr8-unsplash.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  article {
    width: 80%;

    .name {
      color: #d19a66;
      font-size: 20px;
      margin-bottom: 1rem;
    }
    p {
      color: #ffffff;
      font-size: 16px;
    }
  }
}

@media only screen and (min-width: 700px) {
  .hello {
    article {
      .name {
        font-size: 33px;
      }
      p {
        font-size: 19px;
      }
    }
  }
}
</style>
