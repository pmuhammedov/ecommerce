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
  max-width: 1366px;
  width: 100%;
  /* border: 1px solid #dfdfdf; */
  /* position: fixed; */
  z-index: 3;
  background: #ffffff;
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

@media screen and (max-width: 1000px) {
  .search__part {
    max-width: 457px;
  }
  .header__search__input {
    max-width: 420px;
  }
}
@media screen and (max-width: 870px) {
  .search__part {
    max-width: 357px;
  }
  .header__search__input {
    max-width: 320px;
  }
}
@media screen and (max-width: 770px) {
  .search__part {
    max-width: 257px;
  }
  .header__search__input {
    max-width: 220px;
  }
}
@media screen and (max-width: 700px) {
  .search__part {
    display: none;
  }
  .header__top,
  .header__bottom {
    padding: 0 30px 0 30px;
  }
}
@media screen and (max-width: 500px) {
  .header__top,
  .header__bottom {
    padding: 0 10px 0 10px;
  }
}
</style>
