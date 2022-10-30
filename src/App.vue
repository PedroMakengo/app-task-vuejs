<template>
  <div class="app">
    <Header />
    <BackgroundShopNow />
    <main>
      <Brand />
      <ExploreStyles />
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header";
import BackgroundShopNow from "@/components/BackgroundShopNow";
import Brand from "@/components/Brand";
import ExploreStyles from "@/components/ExploreStyles";
export default {
  name: "App",
  components: {
    Header,
    BackgroundShopNow,
    Brand,
    ExploreStyles,
  },
};
</script>

<style></style>
