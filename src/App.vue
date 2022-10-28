<template>
  <div class="app">
    <header>Minhas Tarefas</header>

    <Task />
  </div>
</template>

<script>
import Task from "@/components/Task.vue";
export default {
  name: "App",
  components: {
    Task,
  },
};
</script>

<style>
header {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 80px;
  font-size: 40px;
  color: #fff;
}
</style>
