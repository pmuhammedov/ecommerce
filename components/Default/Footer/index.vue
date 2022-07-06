<template>
  <div class="footer__body">
    <DefaultFooterDetails />
    <DefaultFooterLinks />
  </div>
</template>
<script>
export default {
  name: "Footer",
};
</script>
<style scoped>
.footer__body {
  max-width: 1366px;
  width: 100%;
  height: auto;
  padding: 70px 90px 50px 90px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
@media screen and (max-width: 800px) {
  .footer__body {
    flex-direction: column;
  }
  .details__container {
    margin-bottom: 20px;
  }
}
</style>
