<template>
  <div class="tech-card">
    <div class="tech-card-icon-container">
      <i><slot name="icon"></slot></i>
    </div>
    <slot name="content" class="tech-name"></slot>
  </div>
</template>

<style scoped>
  .tech-card-icon-container {
    display: flex;
    width: 2.1rem;
    height: 2.1rem;
    background-color: var(--vt-c-white);
    border-radius: 8px;
    justify-content: center;
  }
  i {
    display: flex;
    place-items: center;
    place-content: center;
    width: 1.7rem;
  }
  .tech-name{
    color: var(--vt-c-white);
    justify-content: center;
    align-items: center;
    font-size: 0.9rem;
  }
  .tech-card{
    display: flex;
    flex-direction: column;;
    align-items: center;
  }
</style>