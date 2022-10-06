<script setup>
import Card from "./Card.vue";
</script>
<script>
document.title = "Portfolio | Monica M Nikolaisen";

import image1 from "../assets/holidaze.png";
import image2 from "../assets/starwars.png";
import image3 from "../assets/runshoerun.png";

export default {
  data: function () {
    return {
      image1: image1,
      image2: image2,
      image3: image3,
    };
  },
};
</script>

<template>
  <h1>My projects</h1>
  <div class="flex__wrapper">
    <Card>
      <template #image>
        <img :src="image1" />
      </template>

      <template #description>Project Exam 2</template>

      <template #heading>Holidaze</template>

      <template #links>
        <a href="https://github.com/mmunkvold/nexam" target="_blank" rel="noopener">github repo</a
        ><a href="https://magical-holidaze.netlify.app/" target="_blank" rel="noopener">live site</a></template
      >
    </Card>

    <Card>
      <template #image>
        <img :src="image2" />
      </template>

      <template #description>JS Frameworks Course Assignment</template>

      <template #heading>Star Wars Characters</template>

      <template #links>
        <a href="https://github.com/mmunkvold/jsframeworksCA" target="_blank" rel="noopener">github repo</a
        ><a href="https://charactersofstarwars.netlify.app/" target="_blank" rel="noopener">live site</a></template
      >
    </Card>

    <Card>
      <template #image>
        <img :src="image3" />
      </template>

      <template #description>Semester Project 2</template>

      <template #heading>Run Shoe, Run!</template>

      <template #links>
        <div>
          <a href="https://github.com/mmunkvold/runshoerun" target="_blank" rel="noopener">github repo</a>
        </div>
        <div>
          <a href="https://runshoerun.netlify.app/" target="_blank" rel="noopener">live site</a>
        </div>
      </template>
    </Card>
  </div>
</template>

<style scoped>
.flex__wrapper {
  display: flex;
  flex-direction: column;
  max-width: 1280px;
  gap: 2rem;
  margin-top: 5rem;
}

@media (min-width: 1024px) {
  .flex__wrapper {
    flex-direction: row;
  }
}
</style>
