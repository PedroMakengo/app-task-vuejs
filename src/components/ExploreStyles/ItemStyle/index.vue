<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div
    class="bg-style item__style"
    v-for="(item, index) in items"
    :key="index"
    :style="`background-image: url(${item.urlImage})`"
  >
    <div class="ticket">
      <span>{{ item.name }}</span>
      <span>{{ item.qtProduct }}</span>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "ItemStyleSecondary",
  props: {
    items: Array,
  },
};
</script>

<style scoped>
.style__secondary .item__style {
  width: 48%;
  background-repeat: no-repeat;
  background-size: 100%;
  cursor: pointer;
}
</style>
