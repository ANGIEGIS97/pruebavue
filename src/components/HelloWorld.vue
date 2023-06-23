<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1
    class="bg-gradient-to-r from-pink-600 to-sky-400 bg-clip-text text-5xl font-black text-transparent selection:bg-transparent"
  >
    {{ msg }}
  </h1>

  <button
    type="button"
    class="my-6 rounded bg-pink-300 px-4 py-2 transition-all hover:bg-green-300"
    @click="count++"
  >
    La cuenta es: {{ count }}
  </button>
  <p>
    <code class="text-gray-400">components/HelloWorld.vue</code> to test hot
    module replacement.
  </p>
</template>

<style scoped></style>
