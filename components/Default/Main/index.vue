<template>
  <div class="main__container">
    <div class="background__image__wallpaper"></div>
    <div class="main__left__side">
      <div class="left__title">
        <span>GET THE NEW IPHONE 12 PRO</span>
      </div>
      <div class="left__desc">
        <span
          >A transformative triple‑camera system that adds tons of capability
          without complexity</span
        >
      </div>
      <div class="left__links">
        <div class="buy__now__button__container">
          <NuxtLink to="/"><LazyDefaultMainBuynowbutton /></NuxtLink>
        </div>
        <div class="product__advertising__container">
          <NuxtLink to="/"><LazyDefaultMainAdvertising /></NuxtLink>
        </div>
      </div>
    </div>
    <div class="main__right__side">
      <img
        src="/img/main/phones.png"
        alt="phones"
        srcset="/img/main/phones.png"
      />
    </div>
  </div>
</template>
<script>
export default {
  name: "Main",
};
</script>
<style scoped>
.main__container {
  max-width: 1366px;
  width: 100%;
  background-image: url("/img/main/Mask.png");
  background-size: cover;
  height: 596px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  /* margin-top: 173px;
  position: relative;
  z-index: 2; */
}
.background__image__wallpaper {
  max-width: 1366px;
  width: 100%;
  height: 596px;
  background: #000000;
  opacity: 55%;
  position: absolute;
  z-index: 0;
}
.main__left__side,
.main__right__side {
  width: 674px;
  z-index: 5;
  overflow: hidden;
}
.main__left__side {
  display: flex;
  flex-direction: column;
  padding-top: 116px;
  padding-left: 111px;
  overflow: hidden;
}
.main__right__side img {
  max-width: 903px;
  width: 100%;
  height: 620px;
  object-fit: cover;
  object-position: 10% 100%;
  /* z-index: 2; */
}
.left__title span {
  color: #ffffff;
  font-size: 54px;
  font-family: poppins-semibold;
}
.left__links {
  max-width: 415px;
  width: 100%;
  margin-top: 40px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.left__desc {
  color: #ffffff;
  font-size: 1em;
  font-family: roboto-regular;
}
.buy__now__button__container {
  max-width: 137px;
  width: 100%;
}
.product__advertising__container {
  max-width: 270px;
  width: 100%;
  height: 50px;
}

@media screen and (max-width: 1000px) {
  .main__right__side {
    display: none;
  }
  .main__left__side {
    padding: 0;
    justify-content: center;
    align-items: center;
  }
  .main__container {
    justify-content: center;
    align-items: center;
  }
}
@media screen and (max-width: 400px) {
  .left__links {
    flex-direction: column;
  }
}
</style>
