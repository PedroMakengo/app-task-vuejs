<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="product">
    <div class="container">
      <TitleSection title="New Products" />

      <div class="content-products">
        <template v-for="(item, index) in items" :key="index">
          <ProductItem :product="item" />
        </template>
      </div>
    </div>
  </section>
</template>

<script>
import TitleSection from "@/components/TitleSection";
import ProductItem from "@/components/Product/ProductItem";
export default {
  name: "NewProduct",
  data() {
    return {
      items: [
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p1.svg"),
          done: false,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p2.svg"),
          done: false,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p3.svg"),
          done: false,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p4.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p5.svg"),
          done: true,
          promo: "Hot",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p6.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p7.svg"),
          done: false,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../assets/img/product/p8.svg"),
          done: false,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
      ],
    };
  },

  created() {
    console.log(this.items);
  },
  components: {
    TitleSection,
    ProductItem,
  },
};
</script>

<style scoped>
#product {
  padding-block: 4rem;
}

.content-products {
  padding-block: 4rem;
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: space-between;
}
</style>
