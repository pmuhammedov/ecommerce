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
  height: auto;
  display: grid;
  grid-template-columns: auto auto auto auto;
  gap: 25px;
}
@media screen and (max-width: 1000px) {
  .products {
    height: auto;
    grid-template-columns: auto auto;
    justify-content: center;
  }
}
@media screen and (max-width: 600px) {
  .products {
    grid-template-columns: auto;
  }
}
</style>
