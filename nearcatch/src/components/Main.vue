<template>
  <div class="first" style="display: flex; flex-direction: row; align-items: center;">
    <!-- 왼쪽 -->
    <div style="width: 50%;" >
      <!-- 캐러셀 -->
      <div class="carouselArea">
        <div
          id="carouselExampleSlidesOnly"
          class="carousel slide"
          data-bs-ride="carousel"
        >
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img
                src="../assets/휴대폰 화면1.png"
                class="d-block w-100"
                alt="..."
              />
            </div>
            <div class="carousel-item">
              <img
                src="../assets/휴대폰 화면2.png"
                class="d-block w-100"
                alt="..."
              />
            </div>
            <div class="carousel-item">
              <img
                src="../assets/휴대폰 화면3.png"
                class="d-block w-100"
                alt="..."
              />
            </div>
            <!-- <div class="carousel-item">
          <img src="..." class="d-block w-100" alt="..." />
        </div> -->
          </div>
        </div>
      </div>
    </div>
    <!-- 오른쪽 -->
    <div style="width: 50%;">
      <!-- 텍스트 -->
      <div class="firstText">
        <h1 class="text">
          당신의 인연이 궁금하신가요?
        </h1>
        <div>
          <h1 style="display: inline; color: yellow">NearCat:ch Adventure</h1>
          <h1 class="text" style="display: inline">를 다운로드하세요.</h1>
        </div>
        <h5 class="text" style="margin-top: 20px">
          니어캐치 어드벤쳐는 10m 반경 주변 유저와 함께
        </h5>
        <h5 class="text">게임을 즐길 수 있습니다.</h5>
      </div>
      <!-- 앱스토어 이미지 -->
      <div class="appstore">
        <img
          src="../assets/nearcatchAdventureQR.png"
          alt=""
          style="width: 150px"
        />
        <!-- <a href="https://apps.apple.com/kr/app/nearcat-ch/id1630219872">
        <img src="../assets/app-store.png" alt="">
      </a> -->
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "MainView",
};
</script>

<style scoped>
.appstore {
  width: 100%;
  display: flex;
  justify-content: center;
  margin-top: 20px;
  margin-bottom: 20px;
}

.first {
  background-color: rgb(255, 255, 255);
  height: 100vh;
  overflow: hidden;
  background-image: url("../assets/WebBackground.png");
  background-attachment: fixed;
}
.firstText {
  /* display: flex; */
  font-family: "Noto Sans Jp", sans-serif;
  justify-content: center;
  /* margin-top: 70px; */
  text-align: center;
}
.text {
  color: white;
}

.carouselArea {
  /* margin-top: 20%; */
  width: 100%;
  display: flex;
  justify-content: center;
}
.carousel {
  width: 40%;
}
</style>