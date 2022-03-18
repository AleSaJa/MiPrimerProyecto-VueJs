<template>
  <div>
    <h1>Recorrer Arrays con Vue Js</h1>
    <ul>
      <li v-for="color in colores" v-bind:key="color">{{color}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      colores: ['rojo','azul','amarillo','negro']
    }
  }
}
</script>

<style>

</style>
