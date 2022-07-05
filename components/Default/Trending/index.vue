<template>
  <div class="trending">
    <DefaultTrendingTitle />
    <DefaultTrendingProducts />
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
  height: 1050px;
  padding-top: 100px;
  display: flex;
  flex-direction: column;
}
</style>
