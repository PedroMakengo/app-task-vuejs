<template>
  <div class="app">
    <Header />
    <BackgroundShopNow />
    <main>
      <Brand />
      <ExploreStyles />
      <NewProduct />
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header";
import BackgroundShopNow from "@/components/BackgroundShopNow";
import Brand from "@/components/Brand";
import ExploreStyles from "@/components/ExploreStyles";
import NewProduct from "@/components/Product";
export default {
  name: "App",
  components: {
    Header,
    BackgroundShopNow,
    Brand,
    ExploreStyles,
    NewProduct,
  },
};
</script>

<style></style>
