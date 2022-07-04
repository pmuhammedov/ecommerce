<template>
  <div class="new__collection__title">
    <div class="title__top">
      <span>Straight From Nike</span>
    </div>
    <div class="title__bottom">
      <span>New Collection</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "NewcollectionTitle",
};
</script>
<style scoped>
.new__collection__title {
  max-width: 1366px;
  width: 100%;
  height: 60px;
  /* border: 1px solid green; */
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 80px;
}
.title__top span {
  font-size: 0.8em;
  font-family: poppins-regular;
}
.title__bottom span {
  font-size: 1.8em;
  font-family: poppins-semibold;
}
</style>
