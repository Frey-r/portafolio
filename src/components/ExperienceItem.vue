<template>
  <details :open="isOpen">
    <summary class="exp-heading">
      <section class="exp-heading-text">
        <slot name="heading"></slot>
      </section>
      <section class="exp-heading-text-boldest">
        <slot name="heading-boldest"></slot>
      </section>
    </summary>
    <div class="exp-content">
      <slot name="exp-content"></slot>
      <details>
        <summary>
          Principales logros y responsabilidades:
        </summary>
        <ul>
          <slot name="items-achievements"></slot>
        </ul>
      </details>
      <details>
        <summary>
          Tecnologías y herramientas utilizadas:
        </summary>
        <ul>
          <slot name="items-technologies"></slot>
        </ul>
      </details>
    </div>
  </details>
</template>

<style scoped>
  .exp-heading-text{
    color: var(--bt-c-text-secundary);
    font-size: 1.2rem;
  }
  .exp-heading-text-boldest{
    font-variant: all-small-caps;
    color: var(--bt-c-text-primary);
    font-weight: bold !important;
  }
  .exp-heading{
    display: flex;
    flex-direction: column;
  }
  .exp-content{
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
    padding-left: 0.6rem;
  }

</style>
<script setup lang="ts">
defineProps<{
  isOpen?: boolean
}>()
</script>