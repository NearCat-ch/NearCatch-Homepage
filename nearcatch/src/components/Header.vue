<template>
    <!-- 상단 헤더 -->
    <div :class="{'header1': scrollPosition > windowHeight - 70, 'header2': scrollPosition <= windowHeight - 70 }">
        <div class="imgbox">
            <img src="../assets/appstore.png" alt="" class="icon">
        </div>
        <h5 :class="{'content1': scrollPosition > windowHeight - 70, 'content2': scrollPosition <= windowHeight - 70 }">Near Cat:ch</h5>
    </div>
    <!-- 상단 헤더 끝 -->
</template>

<script>
export default {
  name: "HeaderView",
    data: ()=>{
    return {
      scrollPosition: null,
      windowHeight: window.innerHeight,
    }
  },
  methods: {
    updateScroll() {
       this.scrollPosition = window.scrollY
       console.log(this.scrollPosition)
       console.log(this.windowHeight)
    }
  },
  mounted() {
    window.addEventListener('scroll', this.updateScroll);
  }
};
</script>

<style scoped>
    .header1 {
        background-color: rgba(247, 249, 253);
        position: fixed;
        top: 0;
        height: 70px;
        width: 100%;
        z-index: 100;
        display: flex;
        align-items: center;
        /* margin-bottom: 0; */
    }
    .header2 {
        background-color: rgba(255, 255, 255, 0);
        position: fixed;
        top: 0;
        height: 70px;
        width: 100%;
        z-index: 100;
        display: flex;
        align-items: center;
        /* margin-bottom: 0; */
    }
    .imgbox {
        margin-left: 30px;
        width: 30px;
        border-radius: 30%;
        overflow: hidden;
    }
    .icon {
        /* width: 70px; */
        width: 100%;
        object-fit: cover;
    }
    .content1 {
        margin-bottom: 0;
        padding-left: 10px;
    }
    .content2 {
        margin-bottom: 0;
        padding-left: 10px;
        color: rgba(247, 249, 253);
    }
</style>