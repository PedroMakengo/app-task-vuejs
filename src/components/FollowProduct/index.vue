<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section id="brand">
    <div class="container">
      <ul>
        <li v-for="(item, index) in brand" :key="index">
          <img :src="item.image" alt="" />
        </li>
      </ul>
    </div>
  </section>
</template>
