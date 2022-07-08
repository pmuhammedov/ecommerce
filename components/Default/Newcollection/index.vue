<template>
  <div class="new__collection__content">
    <LazyDefaultNewcollectionTitle />
    <LazyDefaultNewcollectionProducts />
    <LazyDefaultRecommendedExplore />
  </div>
</template>
<script>
export default {
  name: "Newcollection",
};
</script>
<style scoped>
.new__collection__content {
  max-width: 1366px;
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-bottom: 30px;
}
</style>
