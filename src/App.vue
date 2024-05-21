<template>
  <div class="layout">
    <div class="layout-left">
      <SideBar />
    </div>
    <div class="layout-right">
      <Banner class="banner" />
      <Paragraphs class="paragraphs" />
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
  height: 1002px;
}

.layout-right {
  width: 1095px;
  height: 1002px;
}

.banner {
  width: 100%;
  height: 634.85px;
}

.paragraphs {
  width: 100%;
  height: 367.15px;
}
</style>
