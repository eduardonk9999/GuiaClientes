<template>
  <div id="app">
    <p>Loop</p>
    <Loops />

    <p>Diretivas</p>
     <Diretiva  :showIdade="true" />
     <Diretiva  :showIdade="false" />
     <Cliente nome="Eduardo"  />
     <hr>
     <br>

    <h1>Guia Clientes</h1>
    <Cliente nome="Eduardo" />
    <Cliente nome="Michael Scott" />
    <hr>
    <Produto />
    <hr>
    <br>
    <br>
    <Props />
    <br>
    <hr>
   
  </div>
</template>

<script>
import Cliente from './components/Cliente'
import Produto from './components/Produto'
import Props from './components/Props'
import Diretiva from './components/DiretivaiF'
import Loops from './components/Loops'


export default {
  name: 'App',
  components: {
    Cliente,
    Produto,
    Props,
    Diretiva,
    Loops,
  }
}
</script>

<style>

</style>
