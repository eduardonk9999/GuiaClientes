<template>
  <div>
    <h2>v-if, v-else</h2>
    <p v-if="showIdade">Condição</p>

    <div :class="{'cliente' : isPremium}">
      <h4>classs com condições</h4>
    </div>
  </div>  
</template>

<script>
  export default {
    data() {
      return {
        isPremium: false

      }
    },
    props: {
      cliente: Object,
      showIdade: Boolean
    }
  }
</script>

<style scoped>
  .cliente {
      color: #552afd;
  }
</style>