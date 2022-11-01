<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="style__secondary">
    <ItemStyle :items="itemsProduct" />
  </div>
</template>

<script>
import ItemStyle from "@/components/ExploreStyles/ItemStyle";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "SecondaryStyle",
  components: { ItemStyle },
  data() {
    return {
      itemsProduct: [
        {
          name: "Item 1",
          qtProduct: 103,
          urlImage: require("../../../assets/img/style/02.svg"),
        },
        {
          name: "Item 2",
          qtProduct: 40,
          urlImage: require("../../../assets/img/style/03.svg"),
        },
        {
          name: "Item 3",
          qtProduct: 70,
          urlImage: require("../../../assets/img/style/04.svg"),
        },
        {
          name: "Item 4",
          qtProduct: 113,
          urlImage: require("../../../assets/img/style/05.svg"),
        },
      ],
    };
  },
};
</script>

<style scoped>
.style__secondary {
  width: 50%;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 1rem;
}
</style>
