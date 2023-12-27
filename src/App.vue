<template>
  <div class="box-border grid h-screen grid-cols-2">
    <div class="p-2 text-center bg-gray-300">
      <input
        v-model="inp1"
        type="text"
        class="w-[50%] py-2 px-2 border border-gray-500 rounded-md"
        placeholder="Send Message ..."
      />
      <p class="p-10 my-2 bg-white rounded-md text-start">{{ inp2 }}</p>
    </div>
    <div class="p-2 text-center">
      <input
        v-model="inp2"
        type="text"
        class="bg-gray-300 w-[50%] py-2 px-2 border rounded-md border-gray-500"
      />
      <p class="p-10 my-2 bg-gray-300 rounded-md text-start">{{ inp1 }}</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const inp1 = ref("Message 1");
const inp2 = ref("Message 2");
</script>

<style scoped></style>
