<template>
  <div class="popular__product">
    <div class="top">
      <div class="discount">
        <span>SALE -50%</span>
      </div>
      <div class="price">
        <span>$99</span>
      </div>
    </div>
    <div class="product__image">
      <img
        src="/img/selectedProduct/NikeAirForceShadow.png"
        alt="NikeAirForceShadow"
      />
    </div>
    <div class="product__name">
      <span>Nike Air Force 1 Shadow</span>
    </div>
    <div class="brand__name">
      <span>Brand: Nike</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "PopularProduct",
};
</script>
<style scoped>
.popular__product {
  max-width: 540px;
  width: 100%;
  height: 680px;
  display: flex;
  flex-direction: column;
  background-color: #f5f5f5;
  border-radius: 10px;
}
</style>
<style scoped>
.top {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 20px 20px 0 20px;
}
.discount > span {
  background: #000000;
  color: #ffffff;
  padding: 7px;
  border-radius: 17px;
  font-size: 0.8em;
  font-family: poppins-medium;
}
.price span {
  font-size: 1em;
  font-family: poppins-medium;
  padding: 6px 16px 6px 16px;
  background: #ffffff;
  border-radius: 17px;
  color: #ff4f04;
}
.product__image {
  margin-top: 10px;
  height: 530px;
}
.product__image img {
  width: 530px;
  height: 520px;
  object-fit: cover;
}
.product__name,
.brand__name {
  padding: 0 20px 0 20px;
}
.product__name span {
  font-size: 1.5em;
  font-family: poppins-semibold;
}
.brand__name span {
  font-size: 0.8em;
  font-family: roboto-regular;
}
</style>
