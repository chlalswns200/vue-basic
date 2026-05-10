<template>
    <h1>과일 반복문</h1>
    <ui>
      <li v-for="item in items">{{ item.fruit }} - {{ item.price }}</li>
    </ui>
</template>

<script>
export default {
  data() {
    return {
      items:[
        {fruit: "딸기" , price:"1,000원"},
        {fruit: "사과" , price:"500원"},
        {fruit: "바나나" , price:"3,000원"},
        {fruit: "수박" , price:"1,5000원"}
      ]
    };
  }
};
</script>
