<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button
      class="border border-emerald-500 px-4 py-2"
      type="button"
      @click="count++"
    >
      count is {{ count }}
    </button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code>
      to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank">
      create-vue
    </a>
    , the official Vue + Vite starter
  </p>

  <p>
    Install
    <a href="https://github.com/vuejs/language-tools" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<script setup lang="ts">
  import {ref} from 'vue';

  defineProps({
    msg: {
      type: String,
      required: true,
    },
  });

  const count = ref(0);
</script>

<style scoped lang="scss">
  h1 {
    @apply text-emerald-500 text-2xl px-4 py-2;
  }

  .card {
    @apply flex flex-col justify-center items-center gap-4 my-10;
  }
</style>
