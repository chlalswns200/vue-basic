<template>
  <h1>{{ fullName }}</h1>
  <button @click="remainName">이름 초기화</button>
  <button @click="changeName">이름 변경</button>
</template>

<script>
export default {
  data() {
    return {
      firstName: "홍",
      lastName: "길동"
    };
  },
  computed: {
    fullName() {
      console.log("Compute 호출")
      return `${this.firstName} ${this.lastName}`
    }
  },
  methods: {
    remainName(){
      console.log("버튼1");
      this.firstName = "홍";
    },
    changeName(){
      console.log("버튼2")
      this.firstName = "김";
    }
  }
};
</script>
