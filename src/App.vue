<template>
  <div class="layout">
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
</script>



<style scoped>
.layout {
  width: 1440px;
  height: 1002px;
  display: flex;
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
