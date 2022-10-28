<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="task">
    <form @submit.prevent="">
      <input type="text" v-model="task" placeholder="Tarefa de hoje?" />
      <button type="submit">Adicionar</button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#task {
  max-width: 700px;
  background: #fff;
  border-radius: 4px;
  padding: 20px;

  margin: 20px auto;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
}

form {
  margin-top: 30px;
  display: flex;
  flex-direction: row;
}

form button {
  cursor: pointer;
  background: #0f5959;
  border: 0;
  border-radius: 4px;
  margin-left: 10px;
  padding: 0 15px;

  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
}

input {
  flex: 1;
  border: 1px solid #eee;
  padding: 6px 10px;
  font-size: 14px;
  outline: none;
}
</style>
