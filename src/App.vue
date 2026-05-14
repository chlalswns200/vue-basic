<template>
  <div>
    <ChildComponent v-bind:title="title" v-bind:subTitle="subTitle"/>
  </div>
</template>

<script>
import ChildComponent from "./components/ch04/04-08.vue";

export default {
  components:{
    ChildComponent,
  },
  data(){
    return {
      title: "부모 컴포넌트에서 작성한 데이터 - title",
      subTitle: "부모 컴포넌트에서 작성한 데이터 - subTitle"
    }
  }
};
</script>
