<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="background-shop-now">
    <div class="container">
      <div class="collections">
        <h1>Collections</h1>
        <p>
          You can explore ans shop many differnt collection from various barands
          here.
        </p>

        <a href="#">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M8 12L8 8C8 5.79086 9.79086 4 12 4V4C14.2091 4 16 5.79086 16 8L16 12"
              stroke="#fff"
              stroke-width="2"
              stroke-linecap="round"
            />
            <path
              d="M3.69435 12.6678C3.83942 10.9269 3.91196 10.0565 4.48605 9.52824C5.06013 9 5.9336 9 7.68053 9H16.3195C18.0664 9 18.9399 9 19.514 9.52824C20.088 10.0565 20.1606 10.9269 20.3057 12.6678L20.8195 18.8339C20.904 19.8474 20.9462 20.3542 20.6491 20.6771C20.352 21 19.8435 21 18.8264 21H5.1736C4.15655 21 3.64802 21 3.35092 20.6771C3.05382 20.3542 3.09605 19.8474 3.18051 18.8339L3.69435 12.6678Z"
              stroke="#fff"
              stroke-width="2"
            />
          </svg>
          Shop Now
        </a>
      </div>

      <img src="@/assets/img/image-product.svg" alt="" />
    </div>
  </section>
</template>

<style scoped>
#background-shop-now {
  background: var(--bg-primary);
  background-image: url("../../assets/img/flores-lateral-direto.svg");
  background-repeat: no-repeat;
  background-position-x: right;
  background-position-y: 160px;
  padding-block: 3rem;
}

#background-shop-now::after {
  content: "";
  display: block;

  background-image: url("../../assets/img/flores-lateral-esquerdo.svg");
  background-repeat: no-repeat;
  width: 500px;
  height: 200px;

  position: absolute;
  top: 60%;
}

#background-shop-now .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

#background-shop-now .container .collections {
  width: 55%;
}

#background-shop-now .container .collections h1 {
  font-size: 4rem;
  font-weight: 100;
}

#background-shop-now .container .collections p {
  font-size: 1.4rem;
  font-weight: 100;
  line-height: 3rem;

  padding-block: 2rem;
}

#background-shop-now .container .collections a {
  background: var(--bg-btn);

  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;

  width: 30%;
  height: 3rem;
  filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));

  color: #fff;
}

#background-shop-now .container img {
  width: 37%;
}
</style>
