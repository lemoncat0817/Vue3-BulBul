<template>
  <div class="header" :class="{ headerOpen: isShow }">
    <div class="headerTop">
      <div class="hamburger" v-if="!isShow" @click="isShow = !isShow">
        <div class="hamburgerLine" />
      </div>
      <div class="hamburgerClose" v-if="isShow" @click="isShow = !isShow">
        <div class="hamburgerCloseLine1" />
        <div class="hamburgerCloseLine2" />
      </div>
      <div class="siteName">白頭翁不吃小米</div>
      <Logo class="layoutLogo" />
    </div>
    <div class="navBox">
      <ul class="nav">
        <li v-for="(item, index) in navText" :key="item.text" @click="toggleActive(index)">
          <a href="JavaScript:;" :class="{ active: activeIndex === index }">
            {{ item.text }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import Logo from '@/components/logo/index.vue'
import { ref } from 'vue'

const isShow = ref(false)

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
.header {
  width: 100vw;
  height: 87.74px;
  box-shadow: 0px 4px 4px 0px #00000040;
  display: flex;
  flex-direction: column;
  transition: height 0.8s ease;
}

.header.headerOpen {
  height: 286.43px;
}

.headerTop {
  height: 87.74px;
  display: flex;
  justify-content: space-between;
}

.hamburger {
  width: 24px;
  height: 18px;
  border-top: 4px solid #000000;
  border-bottom: 4px solid #000000;
  display: flex;
  align-items: center;
  margin: 26.87px 26.38px;
  cursor: pointer;
}

.hamburgerLine {
  width: 15.27px;
  height: 4px;
  background: #000000;
}

.hamburgerClose {
  width: 24px;
  height: 21px;
  margin: 38.87px 26.38px;
  cursor: pointer;
}

.hamburgerCloseLine1 {
  width: 28.69px;
  height: 4px;
  background: #000000;
  border: 4px 0px 0px 0px;
  opacity: 0px;
  transform: rotate(-43.09deg);
}

.hamburgerCloseLine2 {
  width: 28.69px;
  height: 4px;
  background: #000000;
  border: 4px 0px 0px 0px;
  opacity: 0px;
  transform: rotate(43.09deg);
  margin-top: -4px;
}

.siteName {
  font-family: Noto Sans;
  font-size: 20px;
  font-weight: 700;
  line-height: 27.24px;
  text-align: left;
  color: #000000;
  margin: 30.37px 0px;
}

.layoutLogo {
  width: 48.78px;
  height: 48.52px;
  border-radius: 50%;
  box-shadow: 0px 0px 6px 0px #00000040;
  background: #ffffff;
  margin: 19.61px 18.84px;
}

.navBox {
  display: flex;
  justify-content: center;
  margin-top: 4.26px;
  margin-bottom: 45.22px;
}

.nav {
  width: 127px;
  height: 149.21px;
  display: flex;
  flex-direction: column;
  justify-content: center;
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
  font-family: Noto Sans;
  font-size: 18px;
  font-weight: 700;
  line-height: 24.52px;
  text-align: center;
  color: #AA6666;
  text-decoration: underline 2px #AA6666
}
</style>