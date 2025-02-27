<template>
  <h4>
    <slot name="heading"></slot>
  </h4>
  <section class="project-tech-list">
    <slot name="technology"></slot>
  </section>
  <section class="project-description">
    <slot name="link"></slot>
    <slot name="description" class="project-description"></slot>
  </section>
</template>

<style scoped>
  .project-tech-list {
    display: flex;
    gap: 0.6rem;
  }
  .project-description {
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
  }
</style>