<template>
  <h1>{{ count }}</h1>
  <button @click="addCount">카운트증가</button>
</template>

<script>
export default {
  data() {
    return{
      count: 10,
    }
  },
  beforeUpdate(){
    console.log("훅 - beforeUpdate: DOM 반영전",this.count);
    console.log("훅 - beforeupdate: 현재 DOM 값",document.querySelector("h1").textContent);
  },
  updated(){
    console.log("훅 - updated: DOM 업데이트 완료",this.count);
    console.log("훅 - updated: 반영된 DOM 값",document.querySelector("h1").textContent);
  },
  methods: {
    addCount() {
      this.count++;
    }
  }
};
</script>
