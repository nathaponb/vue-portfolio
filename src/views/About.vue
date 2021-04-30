<template>
  <div class="about">
    <header>
      <h1>My name is Natthapon Boonthongkaew</h1>
      <h2>25 year old</h2>
      <h2>Thai nationality</h2>
      <h2>self-taught programmer</h2>
      <h2>📞 (+66) 084-2313735</h2>
      <h2>📧 hellonathapon@gmail.com</h2>
      <h2>Languages/Tools</h2>
      <h4 class="tech">
        💅 Front End: javascript, Typescript, React.js, Vue.js, GraphQL,
        Webpack, babel, HTML, EJS, CSS, SASS
      </h4>
      <h4 class="tech">
        💻 Back End: Node.js, Express.js, .NET CORE/ASP.NET, .NET framework
      </h4>
      <h4 class="tech">
        Databases: mySQL, MSSQL, PostgreSQL, mongoDB, ORM (Entity framework)
      </h4>
    </header>
    <section>
      <h2>What do i know so far as a "Self-taught programmer..?"</h2>
      <p>
        <b>- Fullstack Web Developer</b>, I am fairly good in Fullstack
        Javascript language and its ecosystem
      </p>
      <p><b>- Data analytics</b>, working with python is enjoyable for me</p>
      <p>
        <b>- .NET CORE/ASP.NET</b>, i have been learning C#/.NET recently,
        mostly focus on web development to grain my perspective in this
        particular field
      </p>
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

    <section>
      <h2>My personailty, hobby, interest..?</h2>
      <p>
        I am an Interverted person, i like Cats, raining in the morning with a
        cup of coffee while exploding the universe :) well i mean learning
        something new
      </p>
      <p></p>
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
      h2 {
        margin-bottom: 1rem;
      }
      .tech {
        border-left: 4px solid #42b983;
        font-style: italic;
        padding-left: 1rem;
      }
    }
    section {
      text-align: start;
      margin-bottom: 2rem;
    }
  }
}
</style>
