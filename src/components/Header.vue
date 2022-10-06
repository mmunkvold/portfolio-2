<script>
import image from "../assets/logo.png";

export default {
  data: function () {
    return {
      image: image,
    };
  },
};
</script>

<template>
  <header>
    <div>
      <div class="logo">M</div>
      <p class="site__title">Monica Munkvold Nikolaisen</p>
      <p class="tagline">Frontend Developer - Web Designer</p>
    </div>
    <hr />
  </header>
</template>

<style>
header {
  background: var(--black-soft);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  padding: 1em 0 0;
  text-align: center;
  transition: 250ms ease;
  z-index: 1000;
}

.logo {
  color: grey;
  font: 4rem var(--ff-logo);
  position: absolute;
  top: -25px;
  left: 0;
  right: 0;
}

.site__title {
  text-align: center;
  position: relative;
  color: white;
  font-size: 1.2rem;
  font-family: var(--ff-body);
  text-transform: uppercase;
}

.tagline {
  margin: 0.5em 0 0;
  color: var(--medium-grey-clr);
  font-family: var(--ff-heading), serif;
  font-size: 1em;
}
</style>
