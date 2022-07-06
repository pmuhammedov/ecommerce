<template>
  <div class="footer__links">
    <div class="footer__link__products">
      <h5>Products</h5>
      <span>Trending</span>
      <span>My Account</span>
      <span>Vendors</span>
      <span>Brands</span>
      <span>Storefront</span>
    </div>
    <div class="footer__link__legals">
      <h5>Legals</h5>
      <span>License</span>
      <span>Refund Policy</span>
      <span>About Us</span>
      <span>Contacts</span>
    </div>
    <div class="footer__link__contacts">
      <h5>Contacts</h5>
      <span>Fell free get in touch with us via phone or send us a message</span>
      <span>+1 234 567 89 10</span>
      <span>support@khoomi.com</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "Links",
};
</script>
<style scoped>
.footer__links {
  max-width: 630px;
  width: 100%;
  height: 190px;
  /* border: 1px solid red; */
  display: flex;
  flex-direction: row;
  /* justify-content: space-between;d */
}
.footer__link__products,
.footer__link__legals,
.footer__link__contacts {
  max-width: 160px;
  width: 100%;
  height: auto;
  /* border: 1px solid red; */
  display: flex;
  flex-direction: column;
}
.footer__link__products h5,
.footer__link__legals h5,
.footer__link__contacts h5 {
  font-family: poppins-medium;
  margin-bottom: 18px;
}
.footer__link__products span,
.footer__link__legals span,
.footer__link__contacts span {
  font-family: roboto-regular;
  margin-bottom: 10px;
  /* border: 1px solid green; */
}
.footer__link__contacts {
  max-width: 320px;
}
@media screen and (max-width: 550px) {
  .footer__links {
    flex-direction: column;
    margin-top: 20px;
    /* align-items: center; */
  }
  .footer__link__products,
  .footer__link__legals,
  .footer__link__contacts {
    margin-top: 30px;
  }
}
</style>
