<template>
  <div class="hello">
    <router-link to="/about">
      <img
        src="../assets//optimized-images/blake-connally-B3l0g6HLxr8-unsplash.jpg"
        alt="hello"
      />
      <div class="overlay"></div>
    </router-link>

    <router-link to="/about" class="article">
      <!-- <h2 class="helloworld">&lt; 🚀/&gt;</h2> -->
      <h1 class="name">Nathapon Boonthongkaew</h1>
      <h1 class="thin">
        <span>I am a </span
        ><b>
          <span class="text">{{ value }}</span>
          <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span></b
        >
      </h1>
      <!-- <router-link to="/about" class="btn-wrap">
        <div class="btn">
          MY SKILLS
        </div>
      </router-link> -->
    </router-link>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: () => ({
    value: "",
    arr: [
      "Fullstack Web Developer",
      "Data Analyst",
      "Solfware Engineer",
      "Database manager",
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
      background: linear-gradient(
        rgba(29, 38, 113, 0.6),
        rgba(195, 55, 100, 0.6)
      );
      transition: all 0.3s ease;
    }
  }

  .article {
    z-index: 20;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: calc(100% - 100px);
    text-decoration: none;
    text-shadow: 1px 1px 1px rgba(36, 22, 22, 0.4);
    .helloworld {
      font-size: 1.5rem;
    }
    & > * {
      color: #fff;
      margin: 1rem 0;
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
      font-size: 20px;
    }
  }

  .btn-wrap {
    text-decoration: none;
    text-shadow: none;
    .btn {
      background: #00c58e;
      width: 150px;
      border: none;
      box-shadow: 0 1px 3px 0 rgb(0 0 0 / 10%), 0 1px 2px 0 rgb(0 0 0 / 6%);
      padding: 0.75rem 1.5rem;
      margin: 0 auto;
      font-size: 1rem;
      font-weight: 500;
      border-radius: 0.25rem;
    }
  }
}

@media only screen and (min-width: 700px) {
  .hello {
    .article {
      .helloworld {
        font-size: 1.5rem;
        font-weight: 400;
      }
      .name {
        font-size: 35px;
        font-weight: 700;
      }
      .thin {
        font-size: 30px;
      }
    }

    .btn-wrap {
      text-decoration: none;
      text-shadow: none;
      .btn {
        background: #00c58e;
        width: 150px;
        border: none;
        box-shadow: 0 1px 3px 0 rgb(0 0 0 / 10%), 0 1px 2px 0 rgb(0 0 0 / 6%);
        padding: 0.75rem 1.5rem;
        margin: 0 auto;
        font-size: 1rem;
        font-weight: 500;
        border-radius: 0.25rem;
      }
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
