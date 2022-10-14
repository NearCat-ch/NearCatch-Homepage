<template>
  <div :class="{'second': !first & !second & !third, 'second1':first, 'second2': second,'second3': third }">
    <h1 style="text-align: center; padding-top: 15vh; padding-bottom: 30px">FAQ</h1>
    <div style="width: 100%; display: flex; justify-content: center">
      <div class="FAQ" style="width: 30%">
        <div class="FAQ-list">
          <button class="accordion" @click="togglefirst">
            Q. 니어캐치 어드벤쳐는 누가 만들었나요?
          </button>
          <ul v-if="first">
            <li>
              A. 애플 개발자 아카데미에서 모인 6명의 잘생긴 남자들. Team 2PM이 만들었습니다.
            </li>
          </ul>
          <!-- <div class="panel" >
            <p>내용 1</p>
            </div> -->
        </div>

        <div class="FAQ-list">
          <button class="accordion" @click="togglesecond">
            Q. 로그인이 필요한가요?
          </button>
          <ul v-if="second">
            <li>
                A. 니어캐치 어드벤쳐는 Apple 로그인, 구글 로그인으로 간단하게 로그인하여 즐길 수 있습니다. 
            </li>
          </ul>
        </div>

        <div class="FAQ-list">
          <button class="accordion" @click="togglethird">
            Q. 안전한 서비스 인가요?
          </button>
          <ul v-if="third">
            <li>
              A. 저희 서비스는 개인 정보를 수집하지 않습니다. 특정 기능(주변 기기 탐색을 위한 Nearby interation 등)에 대한 권한만 허용하시면, 저희 서비스를 안전하게 사용할 수 있습니다.
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SecondView",
  data: () => {
    return {
      first: false,
      second: false,
      third: false,
    };
  },
  methods: {
    togglefirst() {
      if (this.first == false) {
        this.first = true;
        this.second = false;
        this.third = false;
      } else {
        this.first = false;
      }
    },
    togglesecond() {
      if (this.second == false) {
        this.first = false;
        this.second = true;
        this.third = false;
      } else {
        this.second = false;
      }
    },
    togglethird() {
      if (this.third == false) {
        this.first = false;
        this.second = false;
        this.third = true;
      } else {
        this.third = false;
      }
    },
  },
};
</script>

<style scoped>
.second {
  background-color: rgba(247, 249, 253);
  height: 70vh;
  /* overflow:auto;  */
  /* display: flex; */
  /* justify-content: center; */
  /* align-items: center; */
  width: 100%;
}

.second1 {
  background-color: rgba(247, 249, 253);
  height: calc(70vh + 42px);
  /* overflow:auto;  */
  /* display: flex; */
  /* justify-content: center; */
  /* align-items: center; */
  width: 100%;
}

.second2 {
  background-color: rgba(247, 249, 253);
  height: calc(70vh + 42px);
  /* overflow:auto;  */
  /* display: flex; */
  /* justify-content: center; */
  /* align-items: center; */
  width: 100%;
}

.second3 {
  background-color: rgba(247, 249, 253);
  height: calc(70vh + 80px);
  /* overflow:auto;  */
  /* display: flex; */
  /* justify-content: center; */
  /* align-items: center; */
  width: 100%;
}

.FAQ {
  text-align: center;
}
.accordion {
  /* background-color: #ffffff; */
  /* box-shadow: 0 0 7px rgb(228, 228, 228);; */
  cursor: pointer;
  /* padding: 16px; */
    height: 50px;
  width: 100%;
  outline: none;
  border: none;
  text-align: center;
  font-size: 15px;
  transition: 0.4s;
}

.accordion-active {
      /* background-color: #ffffff; */
  /* box-shadow: 0 0 7px rgb(228, 228, 228);; */
  cursor: pointer;
  /* padding: 16px; */
    height: 50px;
  width: 100%;
  outline: none;
  border: none;
  text-align: center;
  font-size: 15px;
  transition: 0.4s;
}

.accordion:hover {
  background-color: #f5f5f5;
  font-weight: bold;
}



.panel {
  padding: 0 16px;
  background-color: #ffffff;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
  border-bottom: 1px solid #eeeeee;
}

ul {
  list-style: none;
  padding-left: 0;
  padding-bottom: 20px;
  margin: 0;
  font-size: 14px;
  
}


.FAQ-list {
    /* height: 50px; */
    box-shadow: 0 0 7px rgb(228, 228, 228);;
    margin-bottom: 10px;
    background-color: rgba(255, 255, 255, 0.933);
    border-style: solid rgba(255, 255, 255, 0.933);;
    border-width: 2px;
    border-radius: 5px;
}

li {
    margin: 20px 20px 0px 20px;
}

</style>