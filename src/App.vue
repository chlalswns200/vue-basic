<template>
  <div>
    <h1>isVisible 값: {{ isVisible }}</h1>
    <h1 v-if="isVisible">
      이 문장은 isVisible 값은 {{ isVisible }}일 경우에만 보입니다.
    </h1>

    <button @click="toggleVisibility">버튼</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isVisible: false,
    };
  },
  method: {
    toggleVisibility() {
      this.isVisible = !this.isVisible;
    },
  },
};
</script>
