<template>
  <div class="navs">
    <ul>
      <li>Home</li>
      <li>New</li>
      <li>Arrivals</li>
      <li>Trending</li>
      <li>Deals For You</li>
      <li>Discounts</li>
      <li>Weekly Offers</li>
      <li>Become a Vendor</li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "Navs",
};
</script>
<style scoped>
.navs {
  max-width: 900px;
  width: 100%;
  height: 62.5px;
  margin-left: 70px;
  padding: 0 25px 0 25px;
  /* border: 1px solid green; */
  /* overflow-x: scroll; */
}
ul {
  /* max-width: 900px; */
  /* width: 100%; */
  height: 62.5px;
  list-style: none;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 0;
  margin: 0;
}
li {
  width: auto;
  padding: 18px 20px 18px 20px;
  font-size: 14px;
  font-family: roboto-regular;
}
li:nth-child(1) {
  /* background: red; */
  color: orange;
  border-bottom: 2px solid orange;
}
</style>
