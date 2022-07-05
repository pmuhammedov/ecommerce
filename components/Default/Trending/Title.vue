<template>
  <div class="title__container">
    <div class="top__products">
      <span>TOP PRODUCTS</span>
    </div>
    <div class="trending__product">
      <span>Trending This Week</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "Title",
};
</script>
<style scoped>
.top__products {
  display: flex;
  align-items: center;
  justify-content: center;
}
.trending__product {
  display: flex;
  align-items: center;
  justify-content: center;
}
.top__products span {
  font-size: 0.8em;
  font-family: poppins-regular;
}
.trending__product span {
  font-size: 1.8em;
  font-family: poppins-semibold;
  padding: 0;
}
</style>
