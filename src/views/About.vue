<template>
  <div class="about">
    <header>
      <h1>My name is Natthapon Boonthongkaew</h1>
      <h2>25 year old</h2>
      <h2>🇹🇭 Thai nationality</h2>
      <h2>👨‍💻 self-taught programmer</h2>
      <h2>📞 (+66) 084-2313735</h2>
      <h2>📧 hellonathapon@gmail.com</h2>
      <h2>Languages/Tools</h2>
      <h4>
        💅 Front End: javascript, Typescript, React.js, Vue.js, GraphQL,
        Webpack, babel, HTML, EJS, CSS, SASS
      </h4>
      <h4>
        💻 Back End: Node.js, Express.js, .NET CORE/ASP.NET, .NET framework
      </h4>
      <h4>Databases: mySQL, MSSQL, PostgreSQL, mongoDB</h4>
    </header>
    <section>
      <h2>What do i know so far as a "Self-taught programmer..?"</h2>
      <p>
        <b>- Fullstack Web Developer</b>, I started this journey with HTML and
        CSS 3-4 year ago, with completely new to this field
      </p>
      <p>There are tons of thing i have learned</p>
    </section>

    <section>
      <h2>What about my Education..?"</h2>
      <p>
        I grauated Bechelor degree humanity master in English from
        <a href="https://www.mcu.ac.th/" target="_blank" ref="noreferrer"
          >Mahachulalongkornrajavidyalaya University</a
        >
        in 2019
      </p>
    </section>
  </div>
</template>

<script>
export default {
  name: "About",
};
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
    grid-column: 4 / span 12;
    min-height: 100vh;
    header {
      margin-top: 5rem;
      text-align: start;
      margin-bottom: 1rem;
    }
    section {
      text-align: start;
      margin-bottom: 1rem;
    }
  }
}
</style>
