<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="follow-product">
    <div class="container">
      <TitleSection title="Follow Products And Discounts On Instagram" />

      <div class="content-follow-product">
        <template v-for="(item, index) in items" :key="index">
          <PhotoItem :item="item" />
        </template>
      </div>
    </div>
  </section>
</template>

<script>
import TitleSection from "@/components/TitleSection";
import PhotoItem from "@/components/FollowProduct/PhotoItem";
export default {
  data() {
    return {
      items: [
        {
          to: "/",
          urlImage: require("../../assets/img/photo/photo-1.svg"),
        },
        {
          to: "/",
          urlImage: require("../../assets/img/photo/photo-2.svg"),
        },
        {
          to: "/",
          urlImage: require("../../assets/img/photo/photo-3.svg"),
        },
        {
          to: "/",
          urlImage: require("../../assets/img/photo/photo-4.svg"),
        },
        {
          to: "/",
          urlImage: require("../../assets/img/photo/photo-5.svg"),
        },
        {
          to: "/",
          urlImage: require("../../assets/img/photo/photo-6.svg"),
        },
      ],
    };
  },
  components: {
    TitleSection,
    PhotoItem,
  },
};
</script>

<style scoped>
#follow-product {
  background: #f1f1f1;
  padding-block: 4rem;
}

.content-follow-product {
  display: flex;
  gap: 1rem;
  margin-top: 4rem;
}
</style>
