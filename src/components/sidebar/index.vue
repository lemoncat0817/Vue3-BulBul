<template>
  <div class="sidebar">
    <div class="siteName">白頭翁不吃小米</div>
    <ul class="nav">
      <li v-for="(item, index) in navText" :key="item.text" @click="toggleActive(index)">
        <a href="#" :class="{ active: activeIndex === index }">
          {{ item.text }}
        </a>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from 'vue'

// 預設select白頭翁的特性
const activeIndex = ref(0)
const toggleActive = (index) => {
  // 當前點擊的li，加上active class
  // 其餘的li，移除active class
  // 更新activeIndex的值
  activeIndex.value = activeIndex.value === index ? 0 : index;
};
// nav內容
const navText = ref([{
  text: '白頭翁的特性',
},
{
  text: '白頭翁的故事',
},
{
  text: '白頭翁的美照',
},
{
  text: '白頭翁的危機',
}])

</script>

<style scoped>
.sidebar {
  width: 100%;
  height: 100%;
  background: #FFFFFF;
  box-shadow: 0px 4px 4px 0px #00000040;
  position: relative;
}

.siteName {
  position: absolute;
  width: 210px;
  height: 41px;
  top: 78.33px;
  left: 67.5px;
  gap: 0px;
  opacity: 0px;
  font-family: Noto Sans;
  font-size: 30px;
  font-weight: 700;
  line-height: 40.86px;
  text-align: left;
  color: #000000;
}

.nav {
  position: absolute;
  top: 195px;
  left: 109px;
  gap: 0px;
  opacity: 0px;
}

.nav li {
  display: flex;
  flex-direction: column;
}

.nav li:nth-child(n+2) {
  margin-top: calc(42.74px - 25px);
}

.nav li a {
  width: 127px;
  height: 25px;
  text-decoration: none;
  font-family: Noto Sans;
  font-size: 18px;
  font-weight: 400;
  line-height: 24.52px;
  text-align: center;
  color: #000000;
}

.nav li .active {
  width: 127.15px;
  height: 25px;
  left: -9.75px;
  gap: 0px;
  opacity: 0px;
  font-family: Noto Sans;
  font-size: 18px;
  font-weight: 700;
  line-height: 24.52px;
  text-align: center;
  color: #AA6666;
  text-decoration: underline 2px #AA6666
}
</style>