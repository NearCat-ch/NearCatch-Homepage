<template>
  <div class="footer">
    <div class="foot">
      <h3>Team 2PM</h3>
      <p style="margin:0;">개발자: 이준영, 최원혁, 조현민, 류현선, 김예훈, 황찬기</p>
      <p style="margin:0;">대표 번호 : 010.9582.5604</p>
      <p>대표 이메일 : munam4@naver.com</p>
    </div>

  </div>
</template>

<script>
export default {
  name: "FooterView",
};
</script>

<style scoped>
.footer {
  height: 25vh;
  background-color: rgb(43, 43, 43);
}


.foot {
    padding-top: 30px;
    padding-left: 100px;
    padding-right: 100px;
    color: white;
}

</style>