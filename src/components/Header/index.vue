<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <header id="header">
    <div class="container">
      <div class="header-top">
        <Search />
        <Logo />
        <UserCart />
      </div>
      <Nav />
    </div>
  </header>
</template>

<script>
import Search from "@/components/Search";
import Logo from "@/components/Logo";
import UserCart from "@/components/UserCart";
export default {
  components: {
    Search,
    Logo,
    UserCart,
  },
};
</script>

<style scoped>
#header {
}
</style>
