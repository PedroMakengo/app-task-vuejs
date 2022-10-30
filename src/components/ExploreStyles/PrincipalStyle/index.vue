<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="style__principal"></div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "PrincipalStyle",
};
</script>

<style scoped>
.style__principal::before {
  content: "Explorer New and Popular Styles";
  transform: rotate(-90deg);

  text-transform: uppercase;

  display: block;
  font-weight: 300;
  font-size: 1.45rem;

  position: relative;
  top: 36%;
  left: -55%;
}
</style>
