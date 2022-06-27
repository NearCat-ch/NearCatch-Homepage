<template>
  <div class="second">
    <h1 style="text-align: center;">FAQ</h1>
    <div style="width: 100%; display: flex; justify-content:center;">
      <div class="FAQ" style="width:50%;">
        <div >
            <button class="accordion" @click="togglefirst">니어캐치는 누가 만들었나요?</button>
            <ul v-if="first">
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
  /* align-items: center; */
  width: 100%;
}
.FAQ {
  text-align: center;
}
.accordion {
  background-color: #ffffff;
  cursor: pointer;
  padding: 16px;
  width: 100%;
  outline: none;
  border: none;
  text-align: left;
  font-size: 16px;
  transition: 0.4s;
}

.active,
.accordion:hover {
  background-color: #f5f5f5;
  font-weight: bold;
}

.accordion:after {
  content: "\002B";
  font-weight: bold;
  float: right;
  margin-left: 5px;
}

.active:after {
  content: "\2212";
}

.panel {
  padding: 0 16px;
  background-color: #ffffff;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
  border-bottom: 1px solid #eeeeee;
}
</style>