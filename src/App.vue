<template>
  <div>
    <h1>{{ data }}</h1>
    <h1 v-html="data2"></h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: "오리지널 메세지 데이터",
    //   data2: "<h2 style='color: blue '>HTML 코드 메세지</h2>"
      data2: "<h2 style='color: blue '>HTML 코드 메세지</h2>"
    };
  },
};
</script>
