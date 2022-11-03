<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <footer id="footer">
    <div class="container">
      <h1>Footer</h1>
    </div>
    <Copyright />
  </footer>
</template>

<script>
import Copyright from "../../components/Footer/Copyright";
export default {
  components: { Copyright },
};
</script>

<style scoped>
#footer {
  height: 50vh;

  display: flex;
  flex-direction: column;

  /* padding-block: 4rem; */
}

#footer .container {
  width: 100%;
  height: 90%;

  padding-block: 4rem;
}
</style>
