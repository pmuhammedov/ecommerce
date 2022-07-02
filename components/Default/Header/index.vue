<template>
  <div class="header">
    <div class="header__top">
      <DefaultHeaderLogo />
      <div class="search__part">
        <input
          type="text"
          class="header__search__input"
          placeholder="Search For Products, Brands & Categories"
        />
      </div>
      <DefaultHeaderIcons />
    </div>
    <div class="header__bottom">
      <DefaultHeaderDropdown />
      <DefaultHeaderNav />
    </div>
  </div>
</template>
<script>
export default {
  name: "Header",
};
</script>
<style scoped>
.header {
  height: 173px;
  /* border: 1px solid #dfdfdf; */
}
.header__top {
  height: 110.5px;
  /* border: 1px solid green; */
  display: flex;
  flex-direction: row;
  /* justify-content: baseline; */
  justify-content: space-between;
  align-items: center;
  padding: 0 92px 0 92px;
}

.search__part {
  max-width: 557px;
  width: 100%;
  height: 48px;
  border: 1px solid #dfdfdf;
  border-radius: 10px;
}

.header__search__input {
  max-width: 520px;
  width: 100%;
  height: 100%;
  margin: 0 19px 0 19px;
}
.header__search__input:focus {
  outline: none;
  color: #ababab;
}

.header__bottom {
  height: 62.5px;
  display: flex;
  flex-direction: row;
  align-items: center;
  border-top: 1px solid #dfdfdf;
  padding: 0 92px 0 92px;
}
</style>
