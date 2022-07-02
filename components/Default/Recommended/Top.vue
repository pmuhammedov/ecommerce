<template>
  <div class="recommended__slogan">
    <div>
      <span>Explore Awesome Products</span>
    </div>
    <div><span>Recommended For You</span></div>
  </div>
</template>
<script>
export default {
  name: "RecommendedTop",
};
</script>
<style scoped>
.recommended__slogan {
  display: flex;
  flex-direction: column;
}
.recommended__slogan div:nth-child(1) {
  text-align: center;
}
.recommended__slogan div:nth-child(1) span {
  font-size: 0.8em;
  font-family: poppins-regular;
}
.recommended__slogan div:nth-child(2) span {
  font-size: 1.5em;
  font-family: poppins-semibold;
}
</style>
