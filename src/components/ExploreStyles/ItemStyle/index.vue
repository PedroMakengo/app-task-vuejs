<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div
    class="bg-style item__style"
    v-for="(item, index) in dataExplore"
    :key="index"
    :style="`background: url(${item.urlImage})`"
  >
    <div class="ticket">
      <span>Name</span>
      <span>103 Product</span>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "ItemStyleSecondary",
  props: {
    dataExplore: [],
  },
};
</script>

<style scoped>
.style__secondary .item__style {
  width: 48%;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
