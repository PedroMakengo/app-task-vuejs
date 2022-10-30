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
