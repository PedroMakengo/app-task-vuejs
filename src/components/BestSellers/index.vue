<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="bestSellers">
    <div class="container">
      <TitleSection title="Best Sellers" />
    </div>
  </section>
</template>

<script>
import TitleSection from "@/components/TitleSection";
export default {
  components: {
    TitleSection,
  },
};
</script>

<style scoped>
#bestSellers {
  padding-bottom: 4rem;
}
</style>
