<template>
  <h1>과일 반복문</h1>
  <ul>
    <li v-for="item in items" :key="item.id">
      {{ item.fruit }} - {{ item.price }}
    </li>
  </ul>
  <ul>
    <li v-for="(skill, index) in skills" :key="index">
      {{ skill }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { id: 1, fruit: "딸기", price: "1,000원" },
        { id: 2, fruit: "사과", price: "500원" },
        { id: 3, fruit: "바나나", price: "3,000원" },
        { id: 4, fruit: "수박", price: "15,000원" },
      ],
      skills: [
        "HTML","CSS","Vue.js"
      ]
    };
  },
};
</script>
