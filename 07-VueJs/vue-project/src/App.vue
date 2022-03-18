<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld/>
  <InputVue/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import InputVue from './components/InputVue.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    InputVue
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
