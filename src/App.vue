<script setup lang="ts">
import init, { add } from "rust"
import { ref } from "vue";

const num = ref(0);

init().then(() => {
  num.value = add(1, 2);
})

const handleKeydown = () => {
  console.log("keydown");
}

</script>

<template>
  {{num}}
  <div @click="handleKeydown">123123</div>
</template>

<style scoped></style>
