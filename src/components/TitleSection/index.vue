<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="title-section">
    <h2 class="title">
      {{ title }}
    </h2>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
  },
};
</script>

<style scoped>
#title-section {
  text-align: center;
}

#title-section .title {
  font-family: "Roboto", sans-serif;
  font-size: 2.5rem;
  font-weight: 500;
  text-transform: capitalize;
}
</style>
