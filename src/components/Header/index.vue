<!-- eslint-disable vue/multi-word-component-names -->
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
import Search from "@/components/Header/Search";
import Logo from "@/components/Header/Logo";
import UserCart from "@/components/Header/UserCart";
import Nav from "@/components/Header/Nav";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Header",
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
