<template>
  <div class = project-item>
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
  </div>
</template>

<style scoped>
  .project-item {
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
  }
  h4 {
    color: var(--bt-c-text-primary);
    padding-top:0.6rem;
    font-size: 1.2rem;
  }
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