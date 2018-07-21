<template>
  <div id="app">
  <ul>
    <li v-for="item in Compras">
    {{ item }}
    </li>
    </ul>
  <input type="text" v-model="Message"/>
  <button @click="nomeDaMinhaFuncao()">Botao Teste</button>
  </div>
</template>
<script>
export default {
  name: 'app',
  data: function() {
    return{
      message: 'Lista de Compras',
      Compras: [
        'Pão',
        'Queijo',
        'Mortadela',
        'Maionese',
      ]
    }
  },
  methods: {
    nomeDaMinhaFuncao(){
      alert('kkkk');
    },  
  }
}
</script>
<style>
</style>