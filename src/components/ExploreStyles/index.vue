<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="explore-styles">
    <div class="container">
      <PrincipalStyle />
      <SecondaryStyle />
    </div>
  </section>
</template>

<script>
import PrincipalStyle from "@/components/ExploreStyles/PrincipalStyle";
import SecondaryStyle from "@/components/ExploreStyles/SecondaryStyle";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "ExploreStyles",
  components: { SecondaryStyle, PrincipalStyle },
};
</script>

<style scoped>
#explore-styles {
  padding-bottom: 4rem;
}
#explore-styles .container {
  display: flex;
  justify-content: space-between;
  gap: 1rem;
}

.style__principal {
  background-image: url("../../assets/img/style/01.svg");
  background-repeat: no-repeat;
  background-size: cover;
  width: 50%;
  height: 420px;
}
</style>
