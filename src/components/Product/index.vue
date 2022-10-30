<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="product">
    <div class="container">
      <TitleSection title="New Products" />

      <div class="content-products">
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
        <div class="item-product">
          <div class="bg-item__product bg-product">
            <span>Hot</span>
            <div class="tickets">
              <div class="favorite"></div>
              <a href="#"> Shop Now </a>
            </div>
          </div>
          <div class="content-text">
            <h3>Adicolor Classics joggers</h3>
            <div class="price">
              <span>Dress</span>
              <span>$ 63.85</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import TitleSection from "@/components/TitleSection";
export default {
  name: "NewProduct",
  components: {
    TitleSection,
  },
};
</script>

<style scoped>
#product {
  padding-block: 4rem;
}

.content-products {
  padding-block: 4rem;
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: space-between;
}

.content-products .item-product {
  width: 23.8%;
}

.content-products .bg-product {
  background-color: #ebecec;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 80%;
  height: 35vh;
}

.content-products .item-product:nth-child(1) .bg-item__product {
  background-image: url("../../assets/img/product/p1.svg");
}

.content-products .item-product:nth-child(2) .bg-item__product {
  background-image: url("../../assets/img/product/p2.svg");
}
.content-products .item-product:nth-child(3) .bg-item__product {
  background-image: url("../../assets/img/product/p3.svg");
  background-color: #f1f3f4;
}
.content-products .item-product:nth-child(4) .bg-item__product {
  background-image: url("../../assets/img/product/p4.svg");
  background-color: #f1f3f4;
}
.content-products .item-product:nth-child(5) .bg-item__product {
  background-image: url("../../assets/img/product/p5.svg");
  background-color: #f1f3f4;
}
.content-products .item-product:nth-child(6) .bg-item__product {
  background-image: url("../../assets/img/product/p6.svg");
}
.content-products .item-product:nth-child(7) .bg-item__product {
  background-image: url("../../assets/img/product/p7.svg");
}
</style>
