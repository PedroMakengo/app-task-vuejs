<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <li v-for="(item, index) in items" :key="index">
    <a :href="item.to">{{ item.name }}</a>
  </li>
</template>

<script>
export default {
  props: {
    items: Array,
  },
};
</script>

<style scoped>
a {
  color: var(--text-color-link);

  font-weight: 400;
}

a:hover {
  color: var(--text-color-link-hover);
}
</style>
