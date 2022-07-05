<template>
  <div class="layout__content">
    <div class="layout__main">
      <DefaultHeader />
      <DefaultMain />
      <DefaultRecommended />
      <DefaultShoppingBanner />
      <DefaultNewcollection />
      <DefaultShoppingBanner />
      <DefaultTrending />
      <DefaultShoppingBanner />
      <DefaultFooter />
    </div>
    <slot />
  </div>
</template>
<style scoped>
.layout__content {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  /* border: 1px solid red; */
}
.layout__main {
  max-width: 1366px;
  width: 100%;
  /* border: 1px solid green; */
}
</style>
