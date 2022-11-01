<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <Carousel :items-to-show="4" :wrap-around="true">
    <Slide v-for="(item, index) in items" :key="index">
      <article class="item-product">
        <div
          class="bg-item__product bg-product"
          :class="(active = item.done === false ? 'm-top' : '')"
          :style="`background-image: url(${item.urlImage}) `"
        >
          <span
            v-show="item.done"
            :class="
              (active = item.promo === 'Sale' ? 'activeSale' : 'activeHot')
            "
          >
            {{ item.promo }}
          </span>
          <div class="tickets">
            <div class="content-tickets">
              <div class="favorite">
                <button>
                  <svg
                    width="18"
                    height="18"
                    viewBox="0 0 24 24"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M4.45067 13.9082L11.4033 20.4395C11.6428 20.6644 11.7625 20.7769 11.9037 20.8046C11.9673 20.8171 12.0327 20.8171 12.0963 20.8046C12.2375 20.7769 12.3572 20.6644 12.5967 20.4395L19.5493 13.9082C21.5055 12.0706 21.743 9.0466 20.0978 6.92607L19.7885 6.52734C17.8203 3.99058 13.8696 4.41601 12.4867 7.31365C12.2913 7.72296 11.7087 7.72296 11.5133 7.31365C10.1304 4.41601 6.17972 3.99058 4.21154 6.52735L3.90219 6.92607C2.25695 9.0466 2.4945 12.0706 4.45067 13.9082Z"
                      stroke="#fff"
                      stroke-width="2"
                    />
                  </svg>
                </button>
                <button>
                  <svg
                    width="17"
                    height="17"
                    viewBox="0 0 17 17"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle
                      cx="7"
                      cy="7"
                      r="6"
                      stroke="#fff"
                      stroke-width="2"
                    />
                    <path
                      d="M16 16L13 13"
                      stroke="#fff"
                      stroke-width="2"
                      stroke-linecap="round"
                    />
                  </svg>
                </button>
              </div>
              <button class="shop-now">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M8 12L8 8C8 5.79086 9.79086 4 12 4V4C14.2091 4 16 5.79086 16 8L16 12"
                    stroke="white"
                    stroke-width="2"
                    stroke-linecap="round"
                  />
                  <path
                    d="M3.69435 12.6678C3.83942 10.9269 3.91196 10.0565 4.48605 9.52824C5.06013 9 5.9336 9 7.68053 9H16.3195C18.0664 9 18.9399 9 19.514 9.52824C20.088 10.0565 20.1606 10.9269 20.3057 12.6678L20.8195 18.8339C20.904 19.8474 20.9462 20.3542 20.6491 20.6771C20.352 21 19.8435 21 18.8264 21H5.1736C4.15655 21 3.64802 21 3.35092 20.6771C3.05382 20.3542 3.09605 19.8474 3.18051 18.8339L3.69435 12.6678Z"
                    stroke="white"
                    stroke-width="2"
                  />
                </svg>

                Shop Now
              </button>
            </div>
          </div>
        </div>
        <div class="content-text">
          <h3>Adicolor Classics joggers</h3>
          <div class="price">
            <span class="price-slug">Dress</span>
            <span>$63.85</span>
          </div>
        </div>
      </article>
    </Slide>

    <template #addons>
      <Navigation />
    </template>
  </Carousel>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Navigation, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "WrapAround",
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data() {
    return {
      items: [
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p5.svg"),
          done: true,
          promo: "Hot",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p2.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p4.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
        {
          name: "Adicolor",
          urlImage: require("../../../assets/img/product/p6.svg"),
          done: true,
          promo: "Sale",
          price: 65,
          category: "Dress",
        },
      ],
    };
  },
});
</script>

<style scoped>
.carousel__item {
  background: red;
  width: 95%;
  height: 300px;
}

.bg-item__product {
  height: 35vh;
}
</style>
