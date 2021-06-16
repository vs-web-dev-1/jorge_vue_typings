<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <custom-header
            v-bind:frase-inicial="FRASE"
    ></custom-header>
    <custom-form
            v-bind:frase-inicial="FRASE"
    ></custom-form>
  </div>
</template>

<script>

import CustomHeader from "./components/CustomHeader";
import CustomForm from "./components/CustomForm";
export default {
  name: 'App',
  components: {
    CustomForm,
    CustomHeader
  },
  data: function(){
    return {
      FRASE: 'en un lugar de la mancha',
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
</style>
