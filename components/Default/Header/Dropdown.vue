<template>
  <div class="dropdown__container">
    <button
      id="dropdownDefault"
      @click="toggleDropdown"
      data-dropdown-toggle="dropdownInformation"
      class="dropdown__button text-black hover:bg-gray-300 focus:ring-3 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex items-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
      type="button"
    >
      All Categories
      <svg
        class="w-4 h-4 ml-2"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M19 9l-7 7-7-7"
        ></path>
      </svg>
    </button>
    <!-- Dropdown menu -->
    <div
      id="dropdownInformation"
      class="dropdown__body z-10 hidden bg-white divide-y divide-gray-100 rounded shadow w-44 dark:bg-gray-700"
    >
      <ul
        class="py-1 text-sm text-gray-700 dark:text-gray-200"
        aria-labelledby="dropdownDefault"
      >
        <li>
          <a
            href="#"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
            >Dashboard</a
          >
        </li>
        <li>
          <a
            href="#"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
            >Settings</a
          >
        </li>
        <li>
          <a
            href="#"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
            >Earnings</a
          >
        </li>
        <li>
          <a
            href="#"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
            >Sign out</a
          >
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: "Dropdown",
  methods: {
    async toggleDropdown() {
      const dropdown = document.getElementById("dropdownInformation");
      if (dropdown.classList.contains("hidden")) {
        dropdown.classList.remove("hidden");
      } else {
        dropdown.classList.add("hidden");
      }
    },
  },
};
</script>
<style scoped>
.dropdown__container {
  max-width: 197.49px;
  width: 100%;
  height: 44px;
  /* border: 1px solid red; */
}

.dropdown__button {
  width: 100%;
  background: #f8f8f8;
  border: 1px solid #efefef;
}

.dropdown__body {
  max-width: 197.49px;
  width: 100%;
  position: absolute;
  z-index: 5;
}
</style>
