<template>
  <div class="products">
    <DefaultRecommendedProduct />
    <DefaultRecommendedProduct />
    <DefaultRecommendedProduct />
    <DefaultRecommendedProduct />
  </div>
</template>
<script>
export default {
  name: "Products",
};
</script>
<style scoped>
.products {
  max-width: 1162px;
  width: 100%;
  height: 356px;
  /* border: 1px solid green; */
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
</style>
