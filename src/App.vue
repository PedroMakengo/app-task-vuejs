<template>
  <div class="app">
    <Header />
    <BackgroundShopNow />
    <main>
      <Brand />
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header";
import BackgroundShopNow from "@/components/BackgroundShopNow";
import Brand from "@/components/Brand";
export default {
  name: "App",
  components: {
    Header,
    BackgroundShopNow,
    Brand,
  },
};
</script>

<style></style>
