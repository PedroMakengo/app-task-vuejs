<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <Carousel :items-to-show="4" :wrap-around="true">
    <Slide v-for="(item, index) in items" :key="index">
      <ProductItem :product="item" :class="sliderItem" />
    </Slide>

    <template #addons>
      <Navigation />
    </template>
  </Carousel>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Navigation, Slide } from "vue3-carousel";

import ProductItem from "@/components/Product/ProductItem";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "WrapAround",
  components: {
    Carousel,
    Slide,
    Navigation,
    ProductItem,
  },
  data() {
    return {
      items: [
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p5.svg"),
          done: true,
          promo: "Hot",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p2.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p4.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p6.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
      ],
    };
  },
});
</script>

<style scoped>
.carousel__item {
  width: 95%;
  height: 300px;
}

.bg-item__product {
  height: 50vh;
}

.item-product {
  width: 95%;
}
</style>
