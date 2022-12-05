<template>
  <div id="landing" class="bg-red flex">
    <div id="content">
      <span id="sub" class="text-yellow">Eat pizza everyday</span>
      <span id="full-title" class="text-white">Share your love for pizza</span>
    </div>
    <div id="image">
      <img src="../assets/pizza-full.png" alt="pizza" />
    </div>

  </div>
</template>

<script setup lang="ts">

</script>

<style lang="scss" scoped>
#landing {
  height: 87.3vh;
  width: 100vw;
}
#content {
  overflow: hidden;
  width: 60%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 15rem;
  #sub {
    font-size: 1.8rem;
    font-weight: 800;
  }
  #full-title {
    font-size: 90px;
    font-weight: 900;
    line-height: 1.2;
    text-transform: uppercase;
  }
}
#image {
  width: 40%;
  height: 100%;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding-right: 15rem;
}
</style>
