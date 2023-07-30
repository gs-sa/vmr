<script setup lang="ts">
import init, { add } from "rust"

init().then(() => {
  console.log(add(1, 2))
})

</script>

<template>
  123
</template>

<style scoped></style>
