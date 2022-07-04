<template>
  <div class="banner__content">
    <div class="banner__wallpaper"></div>
    <div class="banner__body">
      <div class="banner__title">
        <span>Sneakers Never Run Out Of Style Get 50% Off Sitewide</span>
      </div>
      <div class="start__shopping">
        <button>Start Shopping</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "ShoppingBanner",
};
</script>
<style scoped>
.banner__content {
  height: 251px;
  background-image: url("~/assets/img/banner/RectangleBanner.png");
  background-size: cover;
  background-position: 80% 70%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.banner__wallpaper {
  max-width: 1366px;
  height: 251px;
  width: 100%;
  position: absolute;
  background: #000000;
  opacity: 53%;
  z-index: 0;
}
.banner__body {
  max-width: 1220px;
  width: 100%;
  height: 106px;
  /* border: 1px solid red; */
  z-index: 1;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.banner__title {
  max-width: 528px;
  width: 100%;
}
.banner__title span {
  color: #ffffff;
  font-size: 35px;
  font-family: poppins-semibold;
}
.start__shopping {
  /* max-width: 224px;
  width: 100%; */
  /* border: 1px solid red; */
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.start__shopping button {
  border: 1px solid #ffffff;
  max-width: 230px;
  width: 100%;
  border-radius: 5px;
  color: #ffffff;
  font-size: 1em;
  font-family: roboto-regular;
  padding: 18px 61px 18px 61px;
}
</style>
