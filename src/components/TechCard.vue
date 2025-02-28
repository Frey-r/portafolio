<template>
  <div class="tech-card">
    <div class="tech-card-icon-container">
      <i><slot name="icon"></slot></i>
    </div>
    <p class="tech-name">
      <slot name="content"></slot>
    </p>
  </div>
</template>

<style scoped>
  .tech-card-icon-container {
    display: flex;
    width: 1.5rem;
    height: 1.5rem;
    background-color: var(--vt-c-white);
    border-radius: 8px;
    justify-content: center;
  }
  i {
    display: flex;
    place-items: center;
    place-content: center;
    width: 1.2rem;
  }
  .tech-name{
    justify-content: center;
    align-items: center;
    font-size: 0.7rem;
  }
  .tech-card{
    display: flex;
    flex-direction: column;;
    align-items: center;
  }
  @media (min-width: 768px) {
    i{
      width: 1.7rem;
    }
    .tech-name{
      font-size: 0.9rem;
    }
    .tech-card-icon-container{
      width: 2.1rem;
      height: 2.1rem;
    }
  }
</style>