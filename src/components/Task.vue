<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="task">
    <form @submit.prevent="addTask">
      <input type="text" v-model="tarefa" placeholder="Tarefa de hoje?" />
      <button type="submit">Adicionar</button>
    </form>

    <TaskItem :lista="tarefas" :delete="deleteTask" />

    <span v-show="tarefas.length > 0"
      >Você têm
      <strong :class="{ pend: pendente }">{{ tarefas.length }}</strong> tarefas
      pendentes</span
    >
  </div>
</template>

<script>
import TaskItem from "@/components/TaskItem.vue";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Task",
  components: {
    TaskItem,
  },
  data() {
    return {
      tarefa: "",
      tarefas: [],
      pendente: false,
    };
  },
  methods: {
    addTask() {
      if (this.tarefa !== "") {
        this.tarefas.push({
          text: this.tarefa,
          key: Date.now(),
        });
      } else {
        alert("Digite uma tarefa...");
        return;
      }
      this.tarefa = "";
      console.log(this.tarefas);
    },
    deleteTask(key) {
      let filtro = this.tarefas.filter(item => {
        return item.key !== key;
      });

      return (this.tarefas = filtro);
    },
  },
  watch: {
    tarefas: {
      deep: true,
      handler() {
        localStorage.setItem("tasks", JSON.stringify(this.tarefas));
        this.tarefas.length > 4
          ? (this.pendente = true)
          : (this.pendente = false);
        console.log("Salvou");
      },
    },
  },
  created() {
    const json = localStorage.getItem("tasks");
    this.tarefas = JSON.parse(json) || [];
  },
};
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

.pend {
  color: #ff0000;
}
</style>
