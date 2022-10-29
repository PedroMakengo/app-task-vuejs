<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="user-cart">
    <a href="#">
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M19.7274 20.4471C19.2716 19.1713 18.2672 18.0439 16.8701 17.2399C15.4729 16.4358 13.7611 16 12 16C10.2389 16 8.52706 16.4358 7.12991 17.2399C5.73276 18.0439 4.72839 19.1713 4.27259 20.4471"
          stroke="#0B0B0B"
          stroke-width="2"
          stroke-linecap="round"
        />
        <circle
          cx="12"
          cy="8"
          r="4"
          stroke="#0B0B0B"
          stroke-width="2"
          stroke-linecap="round"
        />
      </svg>
      Account
    </a>
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
          stroke="#0B0B0B"
          stroke-width="2"
          stroke-linecap="round"
        />
        <path
          d="M3.69435 12.6678C3.83942 10.9269 3.91196 10.0565 4.48605 9.52824C5.06013 9 5.9336 9 7.68053 9H16.3195C18.0664 9 18.9399 9 19.514 9.52824C20.088 10.0565 20.1606 10.9269 20.3057 12.6678L20.8195 18.8339C20.904 19.8474 20.9462 20.3542 20.6491 20.6771C20.352 21 19.8435 21 18.8264 21H5.1736C4.15655 21 3.64802 21 3.35092 20.6771C3.05382 20.3542 3.09605 19.8474 3.18051 18.8339L3.69435 12.6678Z"
          stroke="#0B0B0B"
          stroke-width="2"
        />
      </svg>
      Shopping
    </a>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#user-cart {
  display: flex;
  gap: 1rem;
}

#user-cart a {
  text-decoration: none;

  display: flex;
  font-size: 0.9rem;
  align-items: center;
  gap: 1rem;

  color: #0b0b0b;

  font-weight: 400;
}
</style>
