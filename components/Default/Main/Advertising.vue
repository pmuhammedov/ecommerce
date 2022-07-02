<template>
  <div class="product__advertising">
    <div class="background__wall"></div>
    <div class="advertising__title"><span>With $599 with trade-in</span></div>
  </div>
</template>
<script>
export default {
  name: "Adverting",
};
</script>
<style scoped>
.advertising__title span {
  color: #ffffff;
  /* border: 1px solid green; */
  font-size: 1em;
  padding: 0;
}
.advertising__title {
  width: 236px;
  height: 50px;
  /* border: 1px solid red; */
  padding: 14px 32px 14px 32px;
}
.product__advertising {
  max-width: 236px;
  width: 100%;
}
.background__wall {
  width: 236px;
  height: 50px;
  position: absolute;
  background: #ffffff;
  opacity: 15%;
  border-radius: 5px;
}
</style>
