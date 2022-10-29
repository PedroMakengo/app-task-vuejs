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
import Nav from "@/components/Nav";
export default {
  components: {
    Search,
    Logo,
    UserCart,
    Nav,
  },
};
</script>

<style scoped>
#header {
  background-color: var(--bg-primary);
}

.header-top {
  border-bottom: 1px solid var(--line);

  display: flex;
  justify-content: space-between;

  padding-block: 1.5rem;
}
</style>
