<template>
  <div class="card">
    <div class="image">
      <slot name="image"></slot>
    </div>
    <div class="heading">
      <h2>
        <slot name="heading"></slot>
      </h2>
    </div>
     <div class="description">
      <slot name="description"></slot>
    </div>
    <div class="links">
      <slot name="links"></slot>
    </div>
  </div>
</template>

<style scoped>
.card {
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  max-width: 400px;
  border: 4px solid var(--color-border);
  border-radius: 9px;
  background: var(--black-mute);
  text-align: center;
  padding: 2em;
}

.description{
text-align:left
margin-top:1em
}

.image {
  width: 100%;
  margin: 0 auto 1em;
}
.links {
  display: flex;
  gap: 1em;
  justify-content: center;
}
</style>
