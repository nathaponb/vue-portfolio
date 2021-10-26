<template>
  <div class="about">
    <header>
      <h1>Natthapon Boonthongkaew</h1>
      <h4 class="info">A 25 year old, Thai nationality</h4>
      <h4 class="info">
        UI/UX designer, Fullstack Web Developer, Data Analyst, Database Manager,
        Self-Taught programmer
      </h4>
      <h4 class="info">(+66) 084-2313735</h4>
      <h4 class="info">hellonathapon@gmail.com</h4>
      <h4 class="info">Languages/Tools i know and happy to working with</h4>
      <h4 class="tech">
        💅 Front End: HTML, CSS, SASS, javascript, Typescript, React.js, Vue.js,
        Rest Api, GraphQL, Webpack, babel, git
      </h4>
      <h4 class="tech">
        💻 Back End: Node.js, Express.js, C#/.NET CORE/ASP.NET
      </h4>
      <h4 class="tech">
        💾 Databases: MySQL, MSSQL, PostgreSQL, mongoDB, ORM (Entity framework)
      </h4>
      <h4 class="tech">
        ⭐ Data analytics (Python) with Jupyter Notebook, Numpy, Pandas,
        Mathplotlib, Seaborn
      </h4>
      <h4 class="tech">
        🌟 Design Pattern/Programming Paradigm: MVC, OOP
      </h4>
    </header>
    <section>
      <h2>What do i know so far as a "Self-taught programmer..?"</h2>
      <p>
        <b>- Fullstack Web Developer</b>, I am fairly good in Fullstack
        Javascript and its ecosystem
      </p>
      <p><b>- Data analytics</b>, Jupyter notebook</p>
      <p><b>- C#/.NET CORE/ASP.NET</b>, Intermediate skills</p>
    </section>

    <section>
      <h2>My Education"</h2>
      <p>
        Bachelor degree in Humanity from
        <a href="https://www.mcu.ac.th/" target="_blank" ref="noreferrer"
          >Mahachulalongkornrajavidyalaya University</a
        >, 2019
      </p>
    </section>

    <section>
      <h2>Personality, hobby, interest..?</h2>
      <p>
        Even though i did not guatuated in CS field I am an Self-Taught
        programmer, Enthusiastic person
      </p>
      <p>
        Life is like a cup of Coffee idk lol My hobby is learning new
        Programming Languages, technologies, frameworks and all the related
        thing in this field
      </p>
      <p>
        I am interested in Computer Science, Robotic, Nature, Camping, Astronomy
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
  margin-left: 0;

  header {
    margin-top: 2rem;
    margin-bottom: 4rem;
    text-align: start;
    padding: 1rem;
    background: #f7f9fa;
    border-radius: 8px;

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
    margin-left: 300px;

    min-height: 100vh;
    /* background: #2c3e50; */
    padding: 1rem;
    header {
      margin-top: 0;
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
