<template>
  <div>
    <h1 v-bind:class="className">이렇게 사용해야 해요!</h1>
    <h1 v-bind:class="{active: isActive}">이렇게 사용해야 해요!</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
        className: "title",
        isActive: true,
    };
  },
};
</script>

<style scoped>
h1.active{
    color: green;
}
.title{
    color: orange;
}
</style>
