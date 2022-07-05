<template>
  <div class="products">
    <div class="products__grid__container">
      <DefaultTrendingProduct
        v-for="(product, index) in products"
        :key="index"
        :trendingProduct="product"
      />
    </div>
  </div>
</template>
<script>
export default {
  name: "Products",
  data() {
    return {
      products: [
        {
          title: "Nike Air Force 1",
          image: "/assets/img/products/NikeAirForce.png",
          price: "58",
        },
        {
          title: "NikeCourt Air",
          image: "/assets/img/products/NikeCourtAir.png",
          price: "58",
        },
        {
          title: "Nike SB Zoom",
          image: "/assets/img/products/NikeSbZoom.png",
          price: "58",
        },
        {
          title: "Nike Signal",
          image: "/assets/img/products/NikeSignal.png",
          price: "58",
        },
        {
          title: "Nike Air Force 1",
          image: "/assets/img/products/NikeAirForce.png",
          price: "58",
        },
        {
          title: "NikeCourt Air",
          image: "/assets/img/products/NikeCourtAir.png",
          price: "58",
        },
        {
          title: "Nike SB Zoom",
          image: "/assets/img/products/NikeSbZoom.png",
          price: "58",
        },
        {
          title: "Nike Signal",
          image: "/assets/img/products/NikeSignal.png",
          price: "58",
        },
      ],
    };
  },
};
</script>
<style scoped>
.products {
  max-width: 1366px;
  width: 100%;
  height: 740px;
  padding: 40px 82px 0 82px;
}
.products__grid__container {
  display: grid;
  width: 1200px;
  grid-template-columns: auto auto auto auto;
  gap: 60px 40px;
}
</style>
