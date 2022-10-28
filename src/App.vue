<template>
  <div class="app">
    <h1>Fazer cadastro</h1>

    <div>
      <form @submit.prevent="enviar">
        <label for="">Nome</label>
        <input type="text" v-model="user.nome" /> <br />

        <label for="">Email</label>
        <input type="email" v-model="user.email" /><br />

        <label for="">Qtd Funcionários</label>
        <input type="number" v-model="user.qtFunc" /><br />

        <label for="">Opinião</label>
        <textarea v-model="opiniao"></textarea> <br />

        <label for="">Tecnologias</label>
        <span>
          <input type="checkbox" value="javascript" v-model="tecnologias" />
          JavaScript
        </span>
        <span>
          <input type="checkbox" value="Css" v-model="tecnologias" />
          Css
        </span>
        <span>
          <input type="checkbox" value="VueJs" v-model="tecnologias" />
          VueJs </span
        ><br />

        <label for="">Qual tipo de contratação</label>
        <select v-model="tipoSelecionado">
          <option v-for="item in tipos" :key="item.id" :value="item.nome">
            {{ item.nome }}
          </option>
        </select>
        <br />

        <label for="">Qual seu nível?</label>
        <span><input type="radio" value="basico" v-model="nivel" />Básico</span>
        <span>
          <input type="radio" value="intermediario" v-model="nivel" />
          Intermediário
        </span>
        <span>
          <input type="radio" value="avancado" v-model="nivel" />Avançado
        </span>

        <button type="submit">Enviar</button>
      </form>
    </div>

    <hr />
    <div class="item" v-show="resultado">
      <h2>Usuário cadastrado</h2>

      <label for="">Nome: {{ user.nome }}</label> <br />
      <label for="">Email: {{ user.email }}</label> <br />
      <label for="">Qtd Funcionários : {{ user.qtFunc }}</label> <br />
      <label for="">Sua opinião: {{ opiniao }}</label> <br />
      <label for="">Tecnologias:</label> <br />
      <ul>
        <li v-for="tech in tecnologias" :key="tech">{{ tech }}</li>
      </ul>
      <label>Tipo de Contratação: {{ tipoSelecionado }}</label> <br />
      <label>Nível atual: {{ nivel }}</label> <br />
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      user: {
        nome: "",
        email: "",
        qtdFunc: 0,
      },
      opiniao: "",
      tecnologias: [],
      tipos: [
        { id: 1, nome: "Freelancer" },
        { id: 2, nome: "CLT" },
        { id: 3, nome: "PJ" },
        { id: 4, nome: "Remoto" },
      ],
      tipoSelecionado: "Freelancer",
      nivel: "basico",
      resultado: false,
    };
  },
  methods: {
    enviar() {
      alert("Cadastrado com sucesso");
      this.resultado = true;
    },
  },
};
</script>

<style>
form {
  display: flex;
  flex-direction: column;
}
</style>
