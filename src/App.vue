<template>
  <div class="app">
    <Header />
    <BackgroundShopNow />
    <main>
      <Brand />
      <ExploreStyles />
      <NewProduct />
      <ZaraPromo />
      <BestSellers />
      <FollowProduct />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header";
import BackgroundShopNow from "@/components/BackgroundShopNow";
import Brand from "@/components/Brand";
import ExploreStyles from "@/components/ExploreStyles";
import NewProduct from "@/components/Product";
import ZaraPromo from "@/components/ZaraPromo";
import BestSellers from "@/components/BestSellers";
import FollowProduct from "@/components/FollowProduct";
import Footer from "@/components/Footer";

export default {
  name: "App",
  components: {
    Header,
    BackgroundShopNow,
    Brand,
    ExploreStyles,
    NewProduct,
    ZaraPromo,
    BestSellers,
    FollowProduct,
    Footer,
  },
};
</script>

<style></style>
