<template>
  <section id="abilities" class="section centered">
    <div id="ability-container">
      <!-- Title -->
      <h1 class="h1-dark-bg" style="background-color: var(--dark-purple)">Abilities</h1>
      <p class="quote-purple">"I like to learn. That's an art and a science." - Katherine Johnson</p>
      <!-- Categories -->
      <div v-for="(category, index) in categories" :key="index" class="mb-4">
        <!-- Category Titles -->
        <hr class="horizontal-divider" />
        <div class="d-flex">
          <h2 class="h2-dark-bg mb-3">{{ category.title }}</h2>
        </div>
        <!-- Category Ratings -->
        <div class="row" style="padding: 0; margin: 0">
          <div v-for="(rating, skill) in category.items" :key="skill" class="col-12 col-md-6">
            <AbilityRating :ability="skill" :rating="rating" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import AbilityRating from "../AbilityRating.vue";

const categories = [
  {
    // to do: consider adding sass
    title: "Skills",
    items: {
      "JavaScript/TypeScript": 5,
      "HTML/CSS": 5,
      "Vue.js": 5,
      Bootstrap: 4,
      "React.js": 4,
      Python: 4,
      SQL: 4,
      "C#": 4,
      MongoDB: 3,
      Java: 3,
      Ruby: 2,
      Php: 1,
    },
  },
  {
    title: "Tools",
    items: {
      Git: 5,
      Zoom: 5,
      IntelliJ: 5,
      Slack: 5,
      Figma: 5,
      Atlassian: 5,
      Vitest: 4,
      Cypress: 4,
      VSCode: 4,
      Postman: 4,
      Unity: 3,
      Blender: 2,
    },
  },
  {
    title: "Languages",
    items: {
      English: 5,
      French: 4,
      Spanish: 2,
      "Klingon (qapla’)": 1,
    },
  },
];
</script>

<style scoped lang="scss">
#abilities {
  background-color: var(--dark-purple);
  padding: 4vw 2vw;
}

#ability-container {
  padding: 20px 10px;
  max-width: 900px;
}

.horizontal-divider {
  border-top: 3px solid var(--lightest-purple);
  width: 100%;
  margin: 30px 0;
}

@media (max-width: 768px) {
  .ability-category {
    max-width: 450px;
  }
}
</style>
