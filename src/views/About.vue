<template>
  <div class="about">
    <header>
      <h1>Natthapon Boonthongkaew</h1>
      <h4 class="info">25 year old</h4>
      <h4 class="info">Thai nationality</h4>
      <h4 class="info">self-taught programmer</h4>
      <h4 class="info">📞 (+66) 084-2313735</h4>
      <h4 class="info">📧 hellonathapon@gmail.com</h4>
      <h4 class="info">Languages/Tools</h4>
      <h4 class="tech">
        💅 Front End: HTML, CSS, SASS, javascript, Typescript, React.js, Vue.js,
        GraphQL, Webpack, babel
      </h4>
      <h4 class="tech">
        💻 Back End: Node.js, Express.js, .NET CORE/ASP.NET, .NET framework
      </h4>
      <h4 class="tech">
        💾 Databases: MySQL, MSSQL, PostgreSQL, mongoDB, ORM (Entity framework)
      </h4>
    </header>
    <section>
      <h2>What do i know so far as a "Self-taught programmer..?"</h2>
      <p>
        <b>- Fullstack Web Developer</b>, I am fairly good in Fullstack
        Javascript and its ecosystem
      </p>
      <p><b>- Data analytics</b> with python in Jupyter notebook</p>
      <p>
        <b>- C#/.NET CORE/ASP.NET</b>, i have been learning C#/.NET recently,
        mostly focusing on web development to grain my perspective in this
        particular field
      </p>
    </section>

    <section>
      <h2>What about my Education..?"</h2>
      <p>
        2019, I gratuated Bachelor degree in Humanity master in English from
        <a href="https://www.mcu.ac.th/" target="_blank" ref="noreferrer"
          >Mahachulalongkornrajavidyalaya University</a
        >
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

  header {
    margin-top: 2rem;
    margin-bottom: 4rem;
    text-align: start;
    padding: 0 1rem;

    h1 {
      margin-bottom: 1rem;
    }

    .info {
      text-align: start;
      font-size: 20px;
      margin-bottom: 1rem;
    }
    .tech {
      border-left: 4px solid #42b983;
      font-style: italic;
      padding-left: 1rem;
      font-weight: 500;
    }
  }
  section {
    text-align: start;
    padding: 1rem;
    margin-bottom: 2rem;
    background: #f7f9fa;
    border-radius: 8px;
    h2 {
      margin-bottom: 1rem;
    }
    p {
      line-height: 1.7rem;
    }
  }
}

@media only screen and (min-width: 700px) {
  .about {
    grid-column: 4 / span 12;
    min-height: 100vh;
    header {
      margin-top: 3rem;
      text-align: start;
      margin-bottom: 1rem;
      h2 {
        margin-bottom: 1rem;
      }
    }
    section {
      text-align: start;
      margin-bottom: 2rem;
    }
  }
}
</style>
