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

<style scoped>
#newsletter {
  text-align: center;
}

#newsletter .container h3 {
  font-family: "Roboto", sans-serif;
  font-size: 2.2rem;
  font-weight: 500;
  text-transform: capitalize;
  margin-bottom: 2rem;
}

form {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
}

form input {
  width: 50%;
  border: 0;
  background: none;
  outline: none;
}

form input,
form button {
  padding: 1rem;
  border-bottom: 1px solid var(--text-color-link);
}

form input:focus {
  border-bottom: 1px solid var(--bg-btn) !important;
}

form button {
  text-transform: uppercase;
  font-weight: bold;
}
</style>
