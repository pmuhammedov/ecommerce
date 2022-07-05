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
  height: 350px;
  padding: 70px 90px 50px 90px;
  /* border: 1px solid red; */
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  /* align-items: baseline; */
}
</style>
