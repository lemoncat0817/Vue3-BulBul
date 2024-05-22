<template>
  <div class="logo">
    <div class="bird">
      <div class="birdHeaderTop"></div>
      <div class="birdEye"></div>
      <div class="birdMouth"></div>
      <div class="birdHeaderBottom"></div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.logo {
  width: 100%;
  height: 100%;
  position: relative;
}

.bird {
  width: 100%;
  height: 100%;
  transform: scale(0.8);
}

.birdHeaderTop {
  width: 70%;
  height: 30%;
  background: black;
  position: absolute;
  left: 50%;
  top: 25%;
  transform: translate(-50%, -50%);
  clip-path: polygon(50% 5%, 70% 10%, 85% 30%, 95% 70%, 70% 50%, 50% 45%, 20% 70%, 0% 100%, 10% 60%, 30% 20%);
}

.birdEye {
  width: 12%;
  height: 12%;
  background: black;
  position: absolute;
  left: 58%;
  top: 45%;
  transform: translate(-50%, -50%);
  border-radius: 50%;
}

.birdMouth {
  width: 20%;
  height: 10%;
  background: black;
  position: absolute;
  left: 75%;
  top: 32%;
  transform: translate(-50%, -50%);
  transform: rotate(-10deg);
  border-top-right-radius: 100%;
}

.birdHeaderBottom {
  width: 70%;
  height: 20%;
  background: black;
  position: absolute;
  left: 50%;
  top: 65%;
  transform: translate(-50%, -50%);
  /* 1.上中 6.下中 順時針 */
  clip-path: polygon(55% 40%, 70% 35%, 100% 0%, 85% 55%, 75% 80%, 55% 100%, 35% 100%, 0 100%, 0 40%, 30% 40%);
}
</style>