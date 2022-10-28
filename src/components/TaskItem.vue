<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="item">
    <ul>
      <li v-for="task in lista" :key="task.key">
        <span>{{ task.text }}</span>
        <button @click="deleteItem(task.key)">Concluir</button>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    lista: [],
    delete: Function,
  },
  methods: {
    deleteItem(key) {
      this.delete(key);
    },
  },
};
</script>

<style scoped>
#item {
  white-space: pre-wrap;
  word-wrap: break-word;
}

ul {
  list-style: none;
  padding: 0;
  margin-top: 20px;
}

ul li {
  padding: 15px 0;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}

li:not(:first-child) {
  border-top: 1px solid #eee;
}

span {
  color: #0d2636;
}

button {
  cursor: pointer;
  background: #ddd;
  color: #000;
  border: 0;
  padding: 8px 8px;
  outline: none;
  border-radius: 4px;
}
</style>
