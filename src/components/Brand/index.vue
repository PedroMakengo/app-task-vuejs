<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="brand">
    <div class="container">
      <ul>
        <li v-for="(item, index) in brand" :key="index">
          <img :src="item.image" alt="" />
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Brand",
  data() {
    return {
      brand: [
        { image: require("@/assets/img/brand/brand-1.svg") },
        { image: require("@/assets/img/brand/brand-5.svg") },
        { image: require("@/assets/img/brand/brand-3.svg") },
        { image: require("@/assets/img/brand/brand-4.svg") },
        { image: require("@/assets/img/brand/brand-2.svg") },
      ],
    };
  },
};
</script>

<style scoped>
#brand {
  padding-block: 4rem;
}

#brand ul {
  display: flex;
  justify-content: space-between;
  gap: 1rem;
}
#brand ul li {
  width: 20%;
}

#brand ul li img {
  width: 100%;
}
</style>
