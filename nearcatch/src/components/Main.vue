<template>
  <v-app>

    <!-- 상단 헤더 -->
    <v-app-bar>
      <v-container>
        <v-app-bar-title class="pl-0">
          <div class="d-flex align-center">
            Near Cat:ch
          </div>
        </v-app-bar-title>
      </v-container>
    </v-app-bar>
    <!-- 상단 헤더 끝 -->

    <!-- 메인1 -->
    <v-main>
      <section id="hero">
        <v-sheet
          class="d-flex align-center py-16"
          color="#222222"
          height="420"
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
        </v-sheet>
      </section>
      <!-- 메인1 끝-->


      <!-- 메인2 -->
      <v-sheet>
      </v-sheet>

    </v-main>
  </v-app>
</template>


<script>

export default {
  name: 'MainView',
};
</script>
