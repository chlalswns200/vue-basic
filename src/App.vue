<template>
  <input v-model="email" type="text">

</template>

<script>
export default {
  data() {
    return {
      email: "example@example.com"
    };
  },
  watch:{
    email(newValue,oldValue){
      console.log("newValue",newValue);
      console.log("oldValue",oldValue);
    }
  }
};
</script>
