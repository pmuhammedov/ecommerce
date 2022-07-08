<template>
  <div class="products">
    <div class="left__side">
      <LazyDefaultNewcollectionProduct
        v-for="(product, index) in products"
        :key="index"
        :newProduct="product"
      />
      <!-- <DefaultNewcollectionProduct /> -->
      <!-- <DefaultNewcollectionProduct />
      <DefaultNewcollectionProduct /> -->
    </div>
    <!-- <div class="right__side"> -->
    <LazyDefaultNewcollectionPopularProduct />
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
          image: "NikeAirForce.webp",
          price: "99",
        },
        {
          title: "NikeCourt Air",
          image: "NikeCourtAir.webp",
          price: "99",
        },
        {
          title: "Nike SB Zoom",
          image: "NikeSbZoom.webp",
          price: "99",
        },
        {
          title: "Nike Signal",
          image: "NikeSignal.webp",
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
  height: auto;
  /* border: 1px solid yellow; */
  padding: 52px 128px 0 128px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.left__side {
  max-width: 540px;
  width: 100%;
  height: auto;
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

@media screen and (max-width: 1366px) {
  .products {
    flex-direction: column-reverse;
    justify-content: space-evenly;
    align-items: center;
    padding: 52px 100px 0 100px;
  }
  .left__side {
    margin-top: 30px;
  }
}
@media screen and (max-width: 750px) {
  .products {
    padding: 52px 20px 0 20px;
  }
}
@media screen and (max-width: 600px) {
  .products {
    padding: 52px 60px 0 60px;
  }
  .left__side {
    grid-template-columns: auto;
    justify-content: center;
  }
}
</style>
