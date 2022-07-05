<template>
  <div v-if="newProduct" class="single__product">
    <div class="product__image">
      <img :src="'/img/products/' + newProduct.image" :alt="newProduct.title" />
    </div>
    <div class="product__info">
      <div class="product__title">
        <span>
          {{ newProduct.title }}
        </span>
      </div>
      <div class="product__price">
        <span> ${{ newProduct.price }} </span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Product",
  props: ["newProduct"],
  mounted() {
    // console.log(this.singleProduct);
  },
};
</script>
<style scoped>
.single__product {
  background-color: #f5f5f5;
  max-width: 255px;
  width: 100%;
  height: 313px;
  text-align: center;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: space-between;
  justify-content: space-between;
}
.product__info {
  padding: 0 20.5px 20px 20.5px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: baseline;
}
.product__image img {
  width: 214px;
  height: 214px;
  object-fit: cover;
  margin-left: auto;
  margin-right: auto;
}
.product__title span {
  font-size: 1.2em;
  font-family: poppins-semibold;
}
.product__price span {
  font-size: 1em;
  font-family: poppins-medium;
  padding: 6px 16px 6px 16px;
  background: #ffffff;
  border-radius: 17px;
  color: #ff4f04;
}
</style>
