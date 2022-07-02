<template>
  <div class="recommended__products">
    <div class="recommend__semi__wallpaper"></div>
    <div class="recommended__top"><DefaultRecommendedTop /></div>
    <div class="recommended__bottom">
      <DefaultRecommendedProducts />
      <DefaultRecommendedExplore />
    </div>
  </div>
</template>
<script>
export default {
  name: "Recommended",
};
</script>
<style scoped>
.recommended__products {
  width: 1366px;
  width: 100%;
  height: 676px;
}
.recommend__semi__wallpaper {
  max-width: 1366px;
  width: 100%;
  height: 282px;
  background: #f8f8f8;
  position: absolute;
  z-index: -1;
}
.recommended__top {
  width: 1366px;
  max-width: 100%;
  height: 148px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.recommended__bottom {
  width: 1366px;
  max-width: 100%;
  height: 528px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
