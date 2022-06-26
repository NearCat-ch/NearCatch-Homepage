<template>
  <div class="second">
    <h1 style="text-align: center; magin-top: 100px">FAQ</h1>
    <div style="width: 100%; display:flex; justify-content: center;">
      <div class="FAQ" style="width:50%">
        <div class="rect">
            <button class="accordion" @click="togglefirst">니어캐치는 누가 만들었나요?</button>
            <ul v-if="first" style="margin-bottom: 0;">
                <li>이시발</li>
                <li>좆시발</li>
            </ul>
            <!-- <div class="panel" >
            <p>내용 1</p>
            </div> -->
        </div>


        <button class="accordion" @click="togglesecond">로그인이 필요한가요?</button>
        <div class="panel">
          <p>내용 3</p>
        </div>

        <button class="accordion" @click="togglethird">안전한 서비스 인가요?</button>
        <div class="panel">
          <p>내용 2</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SecondView",
  data: ()=>{
    return {
        first: false,
        second: false,
        third: false,
    }
  },
  methods: {
    togglefirst(){
        if (this.first == false) {
            this.first = true
            this.second = false
            this.third = false
        } else {
            this.first = false
        }
    }, 
    togglesecond(){
        if (this.second == false) {
            this.first = false
            this.second = true
            this.third = false
        } else {
            this.second = false
        }
    },
    togglethird(){
        if (this.third == false) {
            this.first = false
            this.second = false
            this.third = true
        } else {
            this.third = false
        }
    }

  },
};
</script>

<style scoped>
.second {
  height: 100vh;
  /* display: flex; */
  /* justify-content: center; */
  align-items: center;
  width: 100%;
}
.FAQ {
  text-align: center;
}
.rect {
    border: 10px;
    border-color: black;
}


</style>