<template>
  <div>
    <h2>Loops</h2>

    <div v-for="cliente in clientes" :key="cliente.name">
      <h2>{{cliente.nome}}</h2>
      <p>{{cliente.email}}</p>
    </div>
  </div>  
</template>

<script>
  export default {
    data() {
      return {
        clientes: [
          {
            nome: "user",
            email: "user@email.com",
            idade: 99
          },
          {
            nome: "user2",
            email: "user3@email.com",
            idade: 992
          },
          {
            nome: "user3",
            email: "user3@email.com",
            idade: 993
          }
        ]

      }
    },
    props: {
     
    }
  }
</script>

<style scoped>
  
</style>