<template>
  <div id="app">
    <img class="logo" src="./assets/logo.png">
    <Card
      titulo="424"
      descricao="Indicações de lead"
      cor="roxo"
    />
    <Card
      titulo="111"
      descricao="Distribuições de lead"
      cor="verde"
    />
    <Card
      titulo="344"
      descricao="Processos não iniciados"
      cor="azul"
    />
    <Contato 
      nome="Paula"
      idade="24"
      tel="(31)3297-6544"
      msg="teste"
    />
    <Contato 
      :nome="variavel"
      idade="23"
      tel="(31)3297-6544"
      msg="teste2"
    />
    <Contato 
      nome="teste"
      idade="22"
      tel="(31)3297-6544"
      msg="teste3"
    />
   
  </div>
</template>

<script>
import Contato from './components/Contato'
import Card from './components/Card'

export default {
  name: 'App',
  data(){
    return{
      variavel: 'Aa'
    }
  },
  components: {
    Contato,
    Card
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px;   */
}
.logo{
  height: 43px;
  display: block;
}
</style>
