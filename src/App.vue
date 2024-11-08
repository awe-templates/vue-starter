<template>
  <main>
    <div class="logos">
      <a href="https://vitejs.dev" target="_blank">
        <img src="/vite.svg" class="logo" alt="Vite logo" />
      </a>

      <a href="https://vuejs.org/" target="_blank">
        <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
      </a>
    </div>

    <HelloWorld msg="Vite + Vue + TypeScript + Tailwind" />
  </main>
</template>

<script setup lang="ts">
  import HelloWorld from '@/components/HelloWorld.vue';
</script>

<style scoped lang="scss">
  .logos {
    @apply flex flex-row gap-5;

    .logo {
      @apply size-32;

      padding: 1.5em;
      will-change: filter;
      transition: filter 300ms;

      &:hover {
        filter: drop-shadow(0 0 2em #646cffaa);
      }

      &.vue:hover {
        filter: drop-shadow(0 0 2em #42b883aa);
      }
    }
  }
</style>
