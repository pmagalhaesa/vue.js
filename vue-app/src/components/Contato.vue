<template>
  <div class="contato">
    <h1>{{ msg }} Nome:{{ nome }} <br/>Idade:{{ idade }} <br/>Cel: {{ tel }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Contato',
  data () {
    return {
      // msg: 'oi',
    }
  },
  props: {
      nome: String,
      idade: Number,
      tel: Number,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.contato{
  font-size: 10px;
}
</style>
