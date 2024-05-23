<template>
  <div class="banner">
    <div class="bannerImgBox">
      <img class="bannerImg1" src="@/assets/banner/banner.png" alt="Banner">
      <img class="bannerImg2" src="@/assets/banner/banner2.png" alt="Banner">
    </div>
    <div class="title">白頭翁 (Chinese bulbul)</div>
    <div class="subTitle">又名白頭鵯｡以果實﹑昆蟲為主食﹐無法消化小米﹑穀類｡平均壽命約 8~10 年｡</div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.banner {
  width: 100%;
  height: 634.85px;
  background: #0000001A;
  margin-top: 0.64px;
  position: relative;
}

.bannerImgBox {
  margin-top: 0.64px;
  width: 100%;
  height: calc(100% - 0.64px);
  background: #C4C4C4;
}

.bannerImgBox img {
  margin-top: 0.64px;
  width: 100%;
  height: calc(100% - 0.64px);
}


.title {
  position: absolute;
  width: 544px;
  height: 65px;
  right: 44.75px;
  bottom: 65.85px;
  font-family: Noto Sans;
  font-size: 48px;
  font-weight: 700;
  line-height: 65.38px;
  text-align: left;
  color: #FFFFFF;
}

.subTitle {
  position: absolute;
  width: 645px;
  height: 25px;
  right: 44.75px;
  bottom: 36.85px;
  font-family: Noto Sans;
  font-size: 18px;
  font-weight: 400;
  line-height: 24.52px;
  text-align: left;
  color: #FFFFFF;
}

/* 響應式設計 */
/* 768px~1024px */
@media (min-width: 769px) and (max-width: 935px) {
  .title {
    width: 285.28px;
    height: 150px;
    bottom: 83.42px;
    right: 26.95px;
    font-family: Noto Sans;
    font-size: 48px;
    font-weight: 700;
    line-height: 50px;
    text-align: right;
  }
}

/* 1024px以下 */
@media (max-width: 1024px) {
  .subTitle {
    height: 50px;
    width: 329.67px;
    right: 22.67px;
    bottom: 24.07px;
  }
}

/* 768px以上 */
@media (min-width: 769px) {
  .bannerImg2 {
    display: none;
  }
}

/* 768px以下 */
@media (max-width: 768px) {
  .banner {
    height: 311.4px;
  }

  .bannerImgBox {
    margin-top: 0px;
    height: 100%;
  }

  .bannerImg1 {
    display: none;
  }
}

/* 576px以下 */
@media (max-width: 576px) {
  .title {
    width: 285.28px;
    height: 150px;
    bottom: 83.42px;
    right: 26.95px;
    font-family: Noto Sans;
    font-size: 48px;
    font-weight: 700;
    line-height: 50px;
    text-align: right;
  }
}

/* 374px以下 */
@media (max-width: 374px) {
  .subTitle {
    height: 75px;
    width: 289.67px;
    right: 20.67px;
    bottom: 10.07px;
  }
}
</style>