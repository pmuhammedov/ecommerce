<template>
  <div class="new__collection__content">
    <DefaultNewcollectionTitle />
    <DefaultNewcollectionProducts />
    <DefaultRecommendedExplore />
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
  height: 1050px;
  /* border: 1px solid red; */
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
