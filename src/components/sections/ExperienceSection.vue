<template>
  <section id="experience" class="section centered">
    <div id="experience-container">
      <!-- Title and  -->
      <h1 class="h1-dark-bg" style="background-color: var(--dark-purple)">Experience</h1>
      <p class="quote-purple">"Life is either a daring adventure, or nothing at all." - Helen Keller</p>

      <!-- Education -->
      <hr class="horizontal-divider" />
      <div class="d-flex"><h2 class="h2-dark-bg">Education</h2></div>
      <ExperienceEntry
        company="McGill University"
        :startDate="new Date('September 1, 2019')"
        :endDate="new Date('December 31, 2024')"
        position="Double Major in Software Engineering & Psychology, Minor in Educational Psychology"
        description="Notable courses include: Principles of Web Development, Software Design, Modern Computer Games, Database Systems and Algorithms and Data Structures."
        location="Montreal, QB"
        :showTimeAtPosition="false"
      />

      <!-- Work -->
      <hr class="horizontal-divider" />
      <div class="d-flex"><h2 class="h2-dark-bg">Work</h2></div>
      <ExperienceEntry
        company="Perion DOOH"
        :startDate="new Date('March 1, 2025')"
        position="Junior Frontend Developer"
        description="Contributed to the development of Perion's Digital Out of Home (DOOH) ad tech platform using <b>Vue.js</b>, emphasizing user experience and adhering to agile methodologies."
        location="Montreal, QB"
        linkText="Perion DOOH"
        link="https://www.hivestack.com/"
      />
      <ExperienceEntry
        company="Perion DOOH"
        :startDate="new Date('May 1, 2024')"
        :endDate="new Date('December 31, 2024')"
        position="Frontend Intern"
        description="Contributed to the development of Perion's Digital Out of Home (DOOH) ad tech platform using <b>Vue.js</b>, emphasizing user experience and adhering to agile methodologies."
        location="Montreal, QB"
        linkText="Perion DOOH"
        link="https://www.hivestack.com/"
      />
      <ExperienceEntry
        company="Stocate"
        :startDate="new Date('January 1, 2024')"
        :endDate="new Date('May 1, 2024')"
        position="Usability Engineer Intern"
        description="Worked closely with users, gathering and integrating their feedback throughout the entire <b>CI/CD pipeline</b>. Conducted codesign sessions and usability testing to capture insights, and developed <b>Figma</b> prototypes to ensure stakeholder alignment. Iteratively implemented feedback on the Stocate app and website using <b>React</b>, <b>React Native</b>, <b>C#</b>, and <b>PostgreSQL</b>, ensuring seamless deployment and integration across the pipeline."
        location="Montreal, QB"
        linkText="Stocate"
        link="https://www.stocate.com/"
      />
      <ExperienceEntry
        company="Immosquare"
        :startDate="new Date('June 1, 2023')"
        :endDate="new Date('August 1, 2023')"
        position="Junior Web Developer"
        description="As a junior web developer at Immosquare, I learned the basics of web development including <b>HTML</b>, <b>CSS</b>, <b>Bootstrap</b> and <b>JavaScript</b>. I was also introduced to <b>Ruby on Rails</b> and <b>Sequel</b>. During my time at Immosquare I helped to develop and maintain highly functional and visually appealing web pages."
        location="Montreal, QB"
        linkText="Immosquare"
        link="https://immosquare.com/"
      />
    </div>
  </section>
</template>
<script setup>
import ExperienceEntry from "../ExperienceEntry.vue";
</script>
<style scoped lang="scss">
#experience {
  background-color: var(--dark-purple);
  padding: 4vw 2vw;
}

#experience-container {
  padding: 20px 10px;
  width: 100%;
  max-width: 900px;
  text-align: center;
  border-radius: 5px;
}

.horizontal-divider {
  border-top: 3px solid var(--lightest-purple);
  width: 100%;
  margin: 30px 0;
}
</style>
