<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="zara-promo">
    <div class="container">
      <div class="zara-content">
        <img src="@/assets/img/logo.png" alt="" />
        <p>
          Lustrous yet understated. The new evening wear collection exclusively
          offered at the reopened Giorgio Armani boutique in Los Angeles.
        </p>

        <a href="#">See Collection</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#zara-promo {
  background-image: url(../../assets/img/background.png);
  background-repeat: no-repeat;
  background-size: 100%;

  height: 70vh;

  margin-bottom: 4rem;
}

#zara-promo::before {
  content: "";

  background-image: url(../../assets/img/zara-logo.png);
  background-repeat: no-repeat;
  background-size: 100%;

  display: block;

  position: absolute;
  float: right;
  right: 0;
  margin-top: 20px;
  width: 500px;
  height: 400px;
}

.container {
  display: flex;
  height: 100%;
  align-items: center;
  justify-content: flex-end;

  color: white;
}

.container .zara-content {
  width: 50%;
  padding-top: 2rem;
}

.container .zara-content p {
  margin-top: 1rem;
  padding-bottom: 2rem;
  font-size: 1.1rem;
}

.container .zara-content a {
  width: 35%;
  height: 6vh;
  display: flex;
  background: #fff;

  align-items: center;
  justify-content: center;

  color: #000;
}
</style>
