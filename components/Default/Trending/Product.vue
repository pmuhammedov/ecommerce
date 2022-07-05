<template>
  <div v-if="trendingProduct" class="product">
    <div class="trending__image">
      <img :src="'/assets/img/products/' + trendingProduct.image" />
    </div>
    <div class="trending__info">
      <span class="trending__title">{{ trendingProduct.title }}</span>
      <span class="trending__price">${{ trendingProduct.price }}</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "Product",
  props: { trendingProduct: null },
};
</script>
<style scoped>
.product {
  width: 270px;
  height: 310px;
  text-align: center;
  font-size: 30px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  border-radius: 10px;
}
.trending__image img {
  width: 269px;
  height: 269px;
  object-fit: cover;
  border-radius: 10px;
}
.trending__info {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: baseline;
}
.trending__title {
  font-size: 16px;
  font-family: poppins-medium;
}
.trending__price {
  font-size: 14px;
  font-family: poppins-medium;
  background: #ffd881;
  color: #ff4f04;
  padding: 6px 16px 6px 16px;
  border-radius: 17px;
  font-size: 14px;
  font-family: poppins-regular;
}
</style>
