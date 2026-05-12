<template>
  <h1>{{ count }}</h1>
</template>

<script>
export default {
  data() {
    return {
      count: 10
    };
  },
  /* 생성 단계 라이프사이클 */
  beforeCreate(){
    console.log("훅 beforeCreate: 인스턴스 생성 직후 데이터 초기화 전", this.count);
  },
  created(){
    console.log("훅 create: 데이터와 이벤트 모두가 초기화 된 후", this.count);
  }
};
</script>
