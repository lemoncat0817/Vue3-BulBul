<template>
  <div class="paragraphs">
    <div class="paragraphscontent">
      <div class="content">
        <div class="title">外觀
          <div class="decorate"></div>
        </div>
        <div class="text">
          白頭鵯體長約17到22公分﹐額至頭頂純黑色而富有光澤﹐兩眼上方至後枕白色﹐形成一白色枕環｡耳羽後部有一白斑﹐此白環與白斑在黑色的頭部均極為醒目﹐老鳥的枕羽(後頭部)更潔白﹐所以又叫「白頭翁」｡
        </div>
        <div class="text2">
          白頭鵯體長約17到22公分﹐額至頭頂純黑色而富有光澤﹐兩眼上方至後枕白色﹐形成一白色枕環｡耳羽後部有一白斑﹐<br>此白環與白斑在黑色的頭部均極為醒目﹐老鳥的枕羽(後頭部)更潔白﹐所以又叫「白頭<br>翁」｡
        </div>
      </div>
      <div class="contentMid">
        <div class="title">棲地
          <div class="decorate"></div>
        </div>
        <div class="text">
          白頭翁和麻雀﹑綠繡眼合<br>稱「城市三寶」﹐常成群出現在平原區灌木叢﹑丘陵樹林地帶﹐以及校園﹑公園﹑庭院﹑行道中的各種高高的<br>電線與樹上｡
        </div>
        <div class="text2">
          白頭翁和麻雀﹑綠繡眼合<br>稱「城市三寶」﹐常成群出現在平原區灌木叢﹑丘陵樹林地帶﹐以及校園﹑公園﹑庭院﹑行道中的各種高高的電線與樹上｡
        </div>
      </div>
      <div class="content">
        <div class="title">食性
          <div class="decorate"></div>
        </div>
        <div class="text">
          以果樹的漿果和種子為主食﹐並時常飛入果園偷吃果實﹐還會吃嫩葉嫩芽﹐尤其是胡蝶蘭的嫩葉嫩芽葉﹐偶爾啄食昆蟲｡
        </div>
        <div class="text2">
          以果樹的漿果和種子為主食﹐並時常飛入果園偷吃果實﹐還會吃嫩葉嫩芽﹐尤其是胡蝶蘭的嫩葉嫩芽葉﹐偶爾啄食昆<br>蟲｡
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.paragraphs {
  width: 100%;
  height: 367.15px;
  background: #DCCCBC;
  overflow: auto;
}

.paragraphscontent {
  width: 100%;
  height: 225px;
  display: flex;
  justify-content: center;
}

.content {
  width: 278.51px;
  height: 225px;
  display: flex;
  margin: 58.15px 0px 84px 0px;
}

.contentMid {
  width: 278.51px;
  height: 225px;
  display: flex;
  margin: 58.15px 79px 84px 79px;
}

.title {
  width: 36px;
  height: 80px;
  margin: 0px 37.84px 145px 5px;
  font-family: Noto Sans;
  font-size: 36px;
  font-weight: 700;
  line-height: 40px;
  text-align: left;
  color: #000000;
  position: relative;
}

.text {
  width: 199.66px;
  height: 176px;
  font-family: Noto Sans;
  font-size: 16px;
  font-weight: 400;
  line-height: 21.79px;
  text-align: left;
  color: #000000;
}

.text2 {
  width: 223.4px;
  height: 176px;
  font-family: Noto Sans;
  font-size: 16px;
  font-weight: 400;
  line-height: 21.79px;
  text-align: left;
}

.decorate {
  position: absolute;
  width: 10px;
  height: 10px;
  top: 66.58px;
  left: 26.94px;
  gap: 0px;
  border: 8px 0px 0px 0px;
  opacity: 0px;
  border: 8px solid #AA666699;
  border-radius: 60%;
}

/* 響應式設計 */
/* 1360px以下 */
@media (max-width: 1366px) {
  .contentMid {
    margin: 58.15px 50px 84px 50px;
  }
}

/* 1280px以下 */
@media (max-width: 1280px) {
  .contentMid {
    margin: 58.15px 40px 84px 40px;
  }
}

/* 1024px~1280px */
@media (min-width: 1025px) and (max-width: 1279px) {
  .paragraphs {
    height: 557px;
  }

  .paragraphscontent {
    flex-wrap: wrap;
    height: 100%;
    align-items: center;
    justify-content: space-between;
  }

  .content {
    margin: 0px 0px 0px 50.74px;
  }

  .contentMid {
    margin: 0px 50.74px 0px 0px;
  }
}

/* 1024px以下 */
@media (max-width: 1024px) {
  .paragraphs {
    height: 557px;
  }

  .paragraphscontent {
    flex-wrap: wrap;
    height: 100%;
    align-items: center;
    justify-content: space-between;
  }

  .content {
    margin: 0px 0px 0px 50.74px;
  }

  .contentMid {
    margin: 0px 50.74px 0px 0px;
  }
}

/* 769px~1004px */
@media (min-width: 770px) and (max-width: 1003px) {
  .paragraphs {
    height: 641.78px;
  }

  .content:first-child {
    margin: 50.74px 0px 0px 0px;
    height: 176px;
  }

  .content:last-child {
    margin: 0px 0px 50.74px 0px;
    height: 110px;
  }


  .contentMid {
    margin: 50.5px 0px;
    height: 132px;
  }

  .paragraphscontent {
    flex-wrap: nowrap;
    flex-direction: column;
    overflow: hidden;
  }
}

/* 768px以上 */
@media (min-width: 769px) {
  .text2 {
    display: none;
  }
}

/* 768px以下 */
@media (max-width: 768px) {
  .paragraphs {
    height: 604.48px;
    overflow: hidden;
  }

  .content:first-child {
    width: 302.24px;
    height: 176px;
  }

  .content:last-child {
    width: 302.24px;
    height: 110px;
  }

  .contentMid {
    width: 302.24px;
    height: 176px;
  }

  .title {
    margin: 0px 37.84px 96px 5px;
  }

  .text {
    display: none;
  }
}

/* 576px~768px */
@media (min-width: 577px) and (max-width: 767px) {
  .paragraphs {
    height: 641.78px;
  }

  .paragraphscontent {
    justify-content: start;
    flex-direction: column;
    flex-wrap: nowrap;
    align-items: center;
  }

  .content:first-child {
    margin: 50.86px 36.38px 0px 36.38px;
  }

  .content:last-child {
    margin: 0px 36.38px 71.91px 36.38px;
  }

  .contentMid {
    margin: 50.5px 36.38px;
    height: 132px;
  }
}

/* 576px以下 */
@media (max-width: 576px) {
  .paragraphs {
    height: 641.78px;
  }

  .paragraphscontent {
    justify-content: start;
    flex-direction: column;
    flex-wrap: nowrap;
    align-items: center;
  }

  .content:first-child {
    margin: 50.86px 36.38px 0px 36.38px;
  }

  .content:last-child {
    margin: 0px 36.38px 71.91px 36.38px;
  }

  .contentMid {
    margin: 50.5px 36.38px;
    height: 132px;
  }
}
</style>