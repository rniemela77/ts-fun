<script setup lang="ts">
defineProps({
  question: Object,
});

defineEmits(["chooseAnswer"]);
</script>

<template>
  <div>
    <!-- <h1>{{ question.question }}</h1> -->
    <div>
      <button @click="$emit('chooseAnswer', true)">True</button>
      <button @click="$emit('chooseAnswer', false)">False</button>
    </div>
  </div>
</template>

<style></style>
