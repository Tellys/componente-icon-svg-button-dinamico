<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1>Projeto Criação de Componente Dinâmico para Icon Buttom</h1>
  <p>
    <button type="button" class="btn" v-on:click="select()">
      <DinamicButtom icon="logo-conteudo-pertinente" bgColor="#ffffff"> Icon Preto</DinamicButtom>
    </button>
  </p>
  <p>
    <button type="button" class="btn" v-on:click="select()">
      <DinamicButtom icon="logo-conteudo-pertinente" bgColor="silver"> Icon Verde</DinamicButtom>
    </button>
  </p>
  <p>
    <button type="button" class="btn" v-on:click="select()">
      <DinamicButtom icon="logo-conteudo-pertinente" bgColor="yellow"> Icon Verde</DinamicButtom>
    </button>
  </p>
</template>

<script>
import DinamicButtom from '@/components/DinamicButtom.vue';

export default {
  name: 'App',
  components: {
    DinamicButtom
  },
  methods: {
    select() {
      window.location.href = 'https://www.conteudopertinente.com.br/vue3/vue3-criar-componente-icon-svg-button-dinamico-reutilizavel/';
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.btn {
  font-weight: 0;
  font-size: 14px;
  color: #fff;
  background-color: #0066CC;
  padding: 10px 30px;
  border: 2px solid #0066cc;
  box-shadow: rgb(0, 0, 0) 0px 0px 0px 0px;
  border-radius: 5px;
  transition: 1000ms;
  transform: translateY(0);
  align-items: center;
  cursor: pointer;
}

.btn:hover {
  transition: 1000ms;
  padding: 10px 30px;
  transform: translateY(-0px);
  background-color: #fff;
  color: #0066cc;
  border: solid 2px #0066cc;
}
</style>
