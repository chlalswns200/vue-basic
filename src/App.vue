<template>
  <div>
    <h1>프로그래밍 프레임 워크: {{ language }}</h1>
    <h1>Vue를 공부하자</h1>
    <h2>콘텐츠: {{ content }}</h2>
    <h3>작성자: {{author}}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      language: "Vue.js",
      content: "데이터 보관하기",
      author: "홍길동"
    };
  },
};
</script>
