<script setup>
import ProfileComponent from './components/ProfileComponent.vue'
import ThePortfolio from "@/components/ThePortfolio.vue";
</script>

<template class="main-template">

  <header>
    <ProfileComponent />
  </header>
  <main>
    <section class="main-section">
      <ThePortfolio />
    </section>
  </main>

</template>

<style scoped>

header {
  line-height: 1.5;
  position: relative;
}

main {
  margin-top: 0 ;
}

@media (min-width: 1024px) {
  .main-section{
    padding-left: 1.7rem;
  }
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  main {
    overflow-y: scroll;
    overflow-x: clip;
    max-height: 90svh;
    scrollbar-width: none;
  }

  main::-webkit-scrollbar {
    display: none;
  }
}
</style>
