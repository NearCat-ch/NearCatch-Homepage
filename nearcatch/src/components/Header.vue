<template>
    <!-- 상단 헤더 -->
    <div class="header">
        <div class="imgbox">
            <img src="../assets/appstore.png" alt="" class="icon">
        </div>
        <h5 class="content">Near Cat:ch</h5>
    </div>
    <!-- 상단 헤더 끝 -->
</template>

<script>
export default {
  name: "HeaderView",
};
</script>

<style scoped>
    .header {
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
    .content {
        margin-bottom: 0;
        padding-left: 10px;
    }
</style>