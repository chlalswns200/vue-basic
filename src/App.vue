<template>
    <h1>점수는?</h1>
    <h1 v-if="score > 90">Excellent!!</h1>
    <h1 v-else-if="score > 75">Good!</h1>
    <h1 v-else>Needs Improvement.</h1>
</template>

<script>
export default {
  data() {
    return {
      score: 95
    };
  }
};
</script>
