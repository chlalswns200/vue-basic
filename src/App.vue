<template>
  <h1>버튼 이벤트</h1>
  <button @click="handleClick">버튼</button>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods:{
    handleClick(event){
      console.log(event);
      console.log("버튼이 클릭");
    }
  }
};
</script>
