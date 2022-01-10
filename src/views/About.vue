<template>
  <div class="about">
    <header>
      <h1>Nathapon Boontaungkaew</h1>
      <div class="sub-head">
        <h4 class="info en">
          Node.js/Back-end Developer, Python/Data Analysist
        </h4>
        <h4 class="info en">(+66) 084-2313735</h4>
        <h4 class="info en">hellonathapon@gmail.com</h4>
      </div>
      <p class="info">
        My name is Nathapon Boontaungkaew, i am an full-stack web developer, i
        have a solid knowledge of Javascript and its eco-systems. I have a
        intermediate Python skill for Data Analyst
      </p>

      <div class="highlight">
        <h4 class="info">🌟 Why me ?</h4>
        <p class="info">
          Because why not? ¯\_(ツ)_/¯
        </p>
      </div>
      <!-- <div class="highlight">
        <h4 class="info">
          🎓 Education
        </h4>
        <p class="info">
          I grauted bechelor degree at Humanities from
          <a href="https://www.mcu.ac.th/" target="_blank" ref="noreferrer"
            >Mahajulalongkornrajavidyalaya University</a
          >
        </p>
      </div> -->
      <div class="highlight">
        <h4 class="info">
          🥅 เป้าหมายในปีนี้ และในชีวิต
        </h4>
        <p class="info">
          ผมตั้งเป้าหมายของปีนี้ไว้ว่าจะเก่งภาษา Python และ Java ให้ได้
          ทำไมต้องสองภาษานี้ จริงๆผมมีพื้นฐาน Python อยู่บ้างแต่ก็แค่ขั้น
          Beginner และพื้นฐาน Java เพราะสองภาษานี้เป็นภาษาที่มี Field ทางฝั้ง
          back-end ให้ต่อยอดออกไปได้เยอะ ดั่งที่ผมบอกไป ผมไม่ชอบ front-end เลย
          เช่น Python สามารถไปสาย Data Analysis/Data science หรือ Robotic ได้
        </p>
      </div>
      <div class="highlight">
        <h4 class="info">
          🎨 ความสามารถด้านอื่น/บุคลิกส่วนตัว/กิจกรรมยามว่าง
        </h4>
        <p class="info">
          ผมชอบดนตรีแนว LOFI, Country/Indie/Folk
          และตอนนี้ก็กำลังเรียนรู้เรื่องดนตรีอยุ่
          ใครจะรู้บางทีผมอาจผันตัวไปเป็นโปรดิวเซอร์สายนี้ก็เป็นได้
          และอีกอย่างที่ผมสนใจเป็นอย่างมากคือ เรื่อง อวกาศ
          การถ่ายรูปดวงดาวไม่ใช่เรื่องง่ายเลย
          มันต้องอาศัยองค์ประกอบและการเรียนรู้มากมายกว่าจะ สามารถถ่ายออกมาได้
        </p>
      </div>
    </header>
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
    border-radius: 8px;

    .sub-head {
      line-height: 0.7rem;
      margin-bottom: 2rem;
    }

    .highlight {
      background: #f7f9fa;
      padding: 1rem;
      border-radius: 8px;
    }

    h1 {
      margin-bottom: 1rem;
    }

    .info {
      text-align: start;
      font-size: 18px;
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
