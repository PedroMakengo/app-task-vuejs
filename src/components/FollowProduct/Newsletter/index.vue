<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="newsletter">
    <div class="container">
      <h3>Or Subscribe To The Newsletter</h3>

      <form>
        <input type="email" placeholder="Email Address" />
        <button @click.prevent="submitted">Submit</button>
      </form>
    </div>
  </div>
</template>
