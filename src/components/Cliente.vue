<template>
  <div>
    <h2>Data binding</h2>
    <p>{{ nome }}</p>
    <input type="text" :value="nome">

    <hr>
    <br>
    <br>
    <hr>
    <h2>Two way data binding com V-model</h2>
    <input type="text" v-model="nome">
    <p>{{nome}}</p>
    
  </div>
</template>

<script>
  export default {
    data() {
      return {
        numero: '',
        email: '',
        idade: 0
      }
    },
    props: {
      nome: String
    }
  }
</script>


<style scoped>

</style>