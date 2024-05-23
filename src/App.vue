<template>
  <div class="layout">
    <Header class="layoutHeader" />
    <Logo class="layoutLogo" />
    <div class="layout-left">
      <SideBar class="layoutSideBar" />
    </div>
    <div class="layout-right">
      <Banner class="layoutBanner" />
      <Paragraphs class="layoutParagraphs" />
    </div>
  </div>
</template>

<script setup>
import SideBar from './components/sidebar/index.vue'
import Banner from './components/banner/index.vue'
import Paragraphs from './components/paragraphs/index.vue'
import Logo from './components/logo/index.vue'
import Header from './components/header/index.vue'
</script>



<style scoped>
.layout {
  width: 100vw;
  height: 100vh;
}

.layoutHeader {
  width: 100vw;
}

.layoutLogo {
  position: absolute;
  width: 97.56px;
  height: 97.04px;
  top: 47.31px;
  left: 296.22px;
  gap: 0px;
  opacity: 0px;
  z-index: 9999;
  background: #fff;
  box-shadow: 0px 0px 6px 0px #00000040;
  border-radius: 50%;
}

.layout-left {
  width: 345px;
  height: 100%;
}

.layoutSideBar {
  width: 100%;
}

.layout-right {
  width: calc(100vw - 345px);
  height: 100%;
}

/* 響應式設計 */
/* 1024px~1280px */
@media (min-width: 1025px) and (max-width: 1279px) {
  .layoutLogo {
    position: fixed;
  }
}

/* 1024px以下 */
@media (max-width: 1024px) {
  .layoutLogo {
    position: fixed;
  }
}

/* 769以上 */
@media (min-width: 769px) {
  .layoutHeader {
    display: none;
  }

  .layout-right {
    position: absolute;
    left: 345px;
    top: 0;
  }
}

/* 768px以下 */
@media (max-width: 768px) {
  .layout-left {
    display: none;
  }

  .layoutLogo {
    display: none;
  }

  .layout-right {
    width: 100vw;
    left: 0px;
  }
}
</style>
