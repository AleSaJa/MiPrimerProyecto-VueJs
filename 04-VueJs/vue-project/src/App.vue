<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld/>
  <br>
  <lista-de-objeto/>
  <br>
  <div v-for="i in 10" v-bind:key="i">
    <BotonVue/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import ListaDeObjeto from './components/ListaDeObjeto.vue'
import BotonVue from './components/BotonVue.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ListaDeObjeto,
    BotonVue
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
