<template>
  <h1>양방향 바인딩</h1>
  
  <input :value="message" @input="message = $event.target.value">

  <textarea v-model="message"></textarea>

  <input type="checkbox" v-model="checked">

  <input type="radio" value="male" v-model="gender">
  <input type="radio" value="female" v-model="gender">

  <h1>message 입력값: {{ message }}</h1>
  <h1>checked 입력값: {{ checked }}</h1>
  <h1>gender 입력값: {{ gender }}</h1>
</template>

<script>
export default {
  data() {
    return {
      message:"",
      checked: false,
      gender: ""
    };
  }
};
</script>
