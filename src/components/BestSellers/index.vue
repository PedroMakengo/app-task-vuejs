<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="bestSellers">
    <div class="container">
      <TitleSection title="Best Sellers" />

      <div class="content-carousel">
        <Carousel />
      </div>
    </div>
  </section>
</template>

<script>
import TitleSection from "@/components/TitleSection";
import Carousel from "@/components/BestSellers/Carousel";
export default {
  components: {
    TitleSection,
    Carousel,
  },
};
</script>

<style scoped>
#bestSellers {
  padding-bottom: 4rem;
}

.content-carousel {
  margin-top: 3rem;
}
</style>
