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

      <template #description>
        <p>Project Exam 2</p>
        <p> - booking site with contact7enquiry form and an admin area where you can read messages and make changes</p>
        </template>

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

      <template #description>
      <p>JS Frameworks Course Assignment</p>
      <p>- api call to fetch Star Wars Characters and display both all and single result, and login to admin area</p>
      </template>

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

      <template #description>
      <p>Semester Project 2</p>
      <p>- eccommerce site showing shoes from api, a shopping cart and admin area where you can do changes</p>
      </template>

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
