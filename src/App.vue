<template>
  <div>
    <app-header msg="Cadastro TP1"/>
    <cadastro-descricao />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import CadastroDescricao from './components/CadastroDescricao.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    CadastroDescricao
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
</style>
