<template>
  <v-app>
    <v-main>
      <!-- 메인1 -->
      <section class="first">
        <v-sheet
          class="d-flex align-center"
          color="#222222"
          height="100%"
        >
          <v-container>
            <v-responsive width="300">
              <h3 class="text-h3" style="color:white;">
                Near Cat:ch
              </h3>
              <p class="mt-4 text-medium-emphasis" style="color:white;">
                당신의 인연의 별을 찾고 싶으신가요? 니어캐치를 사용해보세요!
              </p>
            </v-responsive>
          </v-container>

          <v-container>
            <v-img
              max-width="200"
              src="../assets/휴대폰 화면1.png"
            />
          </v-container>
        </v-sheet>
      </section>
      <!-- 메인1 끝-->


      <!-- 메인2 -->
      <v-sheet class="second">
        <section id="filter">
          <v-container>
            <v-row justify="space-between">
              <v-col cols="auto">
                <v-responsive width="350">
                  <h2 class="text-h5">
                    당신의 인연을 니어캣이 찾아줄거에요
                  </h2>
                  <p class="mt-3">
                    니어캐치는 여러분이 설정한 관심사를 매칭시킵니다.
                  </p>
                  <p>
                    10m 내에 당신의 인연을 찾으면 생기는 진동을 느껴보세요.
                  </p>


                </v-responsive>
              </v-col>
              <!-- 적절한 이미지 -->
              <v-img
                max-width="250"
                src="../assets/nearcat.png"
              />
            </v-row>
          </v-container>
        </section>
      </v-sheet>

    </v-main>
  </v-app>
</template>


<script>

export default {
  name: 'MainView',
};
</script>

<style scoped>
  .second {
    background-color: rgba(93, 93, 255, 0.424);
  }
  .first {
    height: 100%;
    background-image: "../assets/nearcat.png";
  }
</style>