<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <nav id="nav">
    <ul>
      <ItemNavegator :items="items" />
    </ul>
  </nav>
</template>

<script>
import ItemNavegator from "@/components/ItemNavegator";

export default {
  components: { ItemNavegator },
  data() {
    return {
      items: [
        { to: "/", name: "Jewelry & Accessories" },
        { to: "/clothing", name: "Clothing & Shoes" },
        { to: "/home", name: "Home & Living" },
        { to: "/home", name: "Wedding & Party" },
        { to: "/toys", name: "Toys & Entertainment" },
        { to: "/toys", name: "Art & Collectibles" },
        { to: "/toys", name: "Craft Supplies & Tools" },
      ],
    };
  },
};
</script>

<style scoped>
#nav {
  padding-block: 1rem;
}

#nav ul {
  display: flex;
  justify-content: space-between;
}
</style>
