<template>
  <div class="details__container">
    <div class="footer__logo">
      <img src="~/assets/img/Footer/footer__logo.png" alt="koohi__logo" />
    </div>
    <div class="footer__details">
      <span
        >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore
      </span>
    </div>
  </div>
</template>
<script>
export default {
  name: "Details",
};
</script>
<style scoped>
.details__container {
  max-width: 250px;
  width: 100%;
  height: 155px;
  /* border: 1px solid red; */
  /* margin-top: 50px; */
}
.footer__logo {
  max-width: 250px;
  width: 100%;
}
.footer__logo img {
  max-width: 88px;
  width: 100%;
  height: 59px;
  object-fit: cover;
}
.footer__details {
  max-width: 250px;
  width: 100%;
}
.footer__details span {
  font-size: 16px;
  font-family: roboto-regular;
}
</style>
