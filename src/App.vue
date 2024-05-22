<template>
  <div class="layout">
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
</script>



<style scoped>
.layout {
  width: 1440px;
  height: 1002px;
  display: flex;
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
  height: 100%;
}

.layout-right {
  width: 1095px;
  height: 100%;
}

.layoutBanner {
  width: 100%;
  height: calc(100% - 367.15px);
}

.layoutParagraphs {
  width: 100%;
  height: calc(100% - 634.85px);
}
</style>
