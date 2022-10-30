<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="product">
    <div class="container">
      <TitleSection title="New Products" />
    </div>
  </section>
</template>

<script>
import TitleSection from "@/components/TitleSection";
export default {
  name: "NewProduct",
  components: {
    TitleSection,
  },
};
</script>
