<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="search">
    <button>
      <svg
        width="17"
        height="17"
        viewBox="0 0 17 17"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="7" cy="7" r="6" stroke="#0B0B0B" stroke-width="2" />
        <path
          d="M16 16L13 13"
          stroke="#0B0B0B"
          stroke-width="2"
          stroke-linecap="round"
        />
      </svg>
    </button>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Search",
};
</script>

<style scoped>
#search {
  border: none;
  width: 10%;
}
</style>
