<template>
  <div
    class="text-red-600 flex flex-col justify-center items-center h-full w-full"
  >
    <div>{{ contador }}</div>
    <div class="flex gap-3">
      <button @click="restar">restar</button>
      <button @click="sumar">sumar</button>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
let contador = ref<number>(0);

function sumar() {
  contador.value++;
}

function restar() {
  contador.value--;
}
</script>
