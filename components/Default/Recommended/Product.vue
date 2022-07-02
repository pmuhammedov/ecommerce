<template>
  <div class="product">
    <div>
      <img
        style="border-radius: 10px"
        src="~/assets/img/recommended/Base.png"
        alt="Base"
      />
    </div>
    <div class="product__name">
      <span>Single Tour</span>
    </div>
    <div class="product__price">
      <span>$900</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "Product",
};
</script>
<style scoped>
.product {
  max-width: 270px;
  width: 100%;
  height: 356px;
  /* border: 1px solid red; */
}
.product__name {
  text-align: center;
  padding-top: 17px;
}
.product__name span {
  font-family: poppins-semibold;
  font-size: 1em;
}
.product__price {
  text-align: center;
  padding-top: 15px;
  /* background: #ff4f04; */
}
.product__price span {
  background: #ffd881;
  padding: 8px 13px 6px 13px;
  color: #ff4f04;
  font-family: roboto-medium;
  font-size: 0.8em;
  border-radius: 15px;
}
</style>
