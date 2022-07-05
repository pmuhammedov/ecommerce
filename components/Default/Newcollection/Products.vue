<template>
  <div class="products">
    <div class="left__side">
      <DefaultNewcollectionProduct
        v-for="(product, index) in products"
        :key="index"
        :newProduct="product"
      />
      <!-- <DefaultNewcollectionProduct /> -->
      <!-- <DefaultNewcollectionProduct />
      <DefaultNewcollectionProduct /> -->
    </div>
    <!-- <div class="right__side"> -->
    <DefaultNewcollectionPopularProduct />
    <!-- </div> -->
    <!-- <div class="explore__more">
      <button>Explore Other Products</button>
    </div> -->
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
          image: "~/assets/img/products/NikeAirForce.png",
          price: "99",
        },
        {
          title: "NikeCourt Air",
          image: "~/assets/img/products/NikeCourtAir.png",
          price: "99",
        },
        {
          title: "Nike SB Zoom",
          image: "~/assets/img/products/NikeSbZoom.png",
          price: "99",
        },
        {
          title: "Nike Signal",
          image: "~/assets/img/products/NikeSignal.png",
          price: "99",
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
  /* border: 1px solid yellow; */
  padding: 52px 128px 0 128px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.left__side {
  max-width: 540px;
  width: 100%;
  height: 680px;
  display: grid;
  gap: 50px 30px;
  grid-template-columns: auto auto;
}
.right__side {
  max-width: 540px;
  width: 100%;
  height: 680px;
  border: 1px solid red;
}
.explore__more {
}
</style>
