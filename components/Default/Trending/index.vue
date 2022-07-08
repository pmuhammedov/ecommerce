<template>
  <div class="trending">
    <LazyDefaultTrendingTitle />
    <LazyDefaultTrendingProducts />
  </div>
</template>
<script>
export default {
  name: "Trending",
};
</script>
<style scoped>
.trending {
  max-width: 1366px;
  width: 100%;
  height: auto;
  padding-top: 100px;
  padding-bottom: 30px;
  display: flex;
  flex-direction: column;
}
</style>
