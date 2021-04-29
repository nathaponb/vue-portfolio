<template>
  <div class="hello">
    <router-link to="/about">
      <img src="../assets/pexels-photo-1714207.jpeg" alt="hello" />
      <div class="overlay"></div>
    </router-link>

    <article>
      <h2>Hello World 🚀</h2>
      <h1 class="name">My name is Nathapon Boontaungkaew</h1>
      <h2>25 year old Fullstack Web developer</h2>
      <h1 class="thin">
        <span>I Familiar with </span
        ><b>
          <span class="text">{{ value }}</span>
          <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span></b
        >
      </h1>
    </article>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: () => ({
    value: "",
    arr: [
      "Javascript/Typescript",
      "React.js/Vue.js",
      "Node.js/Express.js",
      "mySQL/PostgreSQL/mongoDB",
      "C#/ASP.NET",
    ],
    charIndex: 0,
    arrIndex: 0,
    typeStatus: false,
    typeSpeed: 100,
    eraseSpeed: 50,
    newValDelay: 2000,
  }),
  methods: {
    // push word in value char by char
    typeText() {
      if (this.charIndex < this.arr[this.arrIndex].length) {
        if (!this.typeStatus) {
          this.typeStatus = true;
        }
        this.value += this.arr[this.arrIndex].charAt(this.charIndex);
        this.charIndex++;
        setTimeout(this.typeText, this.typeSpeed);
      } else {
        this.typeStatus = false;
        setTimeout(this.eraseText, this.newValDelay); // setTimeout(cb, time)
      }
    },
    // erease word char and ++ arr length for new one
    eraseText() {
      if (this.charIndex > 0) {
        if (!this.typeStatus) {
          this.typeStatus = true;
        }
        this.value = this.arr[this.arrIndex].substring(0, this.charIndex - 1);
        this.charIndex -= 1;
        setTimeout(this.eraseText, this.eraseSpeed);
      } else {
        this.typeStatus = false;
        this.arrIndex += 1;
        if (this.arrIndex >= this.arr.length) {
          this.arrIndex = 0;
        }
        setTimeout(this.typeText, this.eraseSpeed);
      }
    },
  },
  created() {
    setTimeout(this.typeText, this.newValDelay + 200);
  },
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

  a {
    overflow: hidden;
    img {
      object-fit: cover;
      object-position: center;
      height: 100%;
      width: 100%;
    }
    .overlay {
      z-index: 10;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.5);
      transition: all 0.3s ease;
    }
  }

  article {
    z-index: 20;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: calc(100% - 100px);
    /* background:crimson; */
    & > * {
      color: #fff;
    }
    h1 {
      .cursor {
        display: inline-block;
        margin-left: 3px;
        width: 4px;
        background-color: #fff;
        animation: cursorBlink 1s infinite;
      }
      .cursor.typing {
        animation: none;
      }
    }
    .name {
      font-weight: 300;
      font-size: 30px;
    }
    .thin {
      font-weight: 300;
    }
  }
}

@keyframes cursorBlink {
  49% {
    background-color: #fff;
  }
  50% {
    background-color: transparent;
  }
  99% {
    background-color: transparent;
  }
}
</style>
