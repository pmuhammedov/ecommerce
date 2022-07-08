<template>
  <div class="products">
    <div class="products__grid__container">
      <LazyDefaultTrendingProduct
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
          image: "NikeAirForce.png",
          price: "58",
        },
        {
          title: "NikeCourt Air",
          image: "NikeCourtAir.png",
          price: "58",
        },
        {
          title: "Nike SB Zoom",
          image: "NikeSbZoom.png",
          price: "58",
        },
        {
          title: "Nike Signal",
          image: "NikeSignal.png",
          price: "58",
        },
        {
          title: "Nike Air Force 1",
          image: "NikeAirForce.png",
          price: "58",
        },
        {
          title: "NikeCourt Air",
          image: "NikeCourtAir.png",
          price: "58",
        },
        {
          title: "Nike SB Zoom",
          image: "NikeSbZoom.png",
          price: "58",
        },
        {
          title: "Nike Signal",
          image: "NikeSignal.png",
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
  height: auto;
  padding-top: 40px;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.products__grid__container {
  display: grid;
  width: 1200px;
  grid-template-columns: auto auto auto auto;
  gap: 60px 40px;
}
@media screen and (max-width: 1250px) {
  .products__grid__container {
    grid-template-columns: auto auto;
    justify-content: center;
  }
}
@media screen and (max-width: 600px) {
  .products__grid__container {
    grid-template-columns: auto;
  }
}
</style>
