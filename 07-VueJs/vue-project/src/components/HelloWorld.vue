<template>
  <div class="card">
    <h5 class="card-header">Featured -> {{opcion}}</h5>
    <div class="card-body">
      <h5 class="card-title">Special title treatment</h5>
      <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
      <a href="#" class="btn btn-primary" v-on:click="opcion = 'Nueva Opción'">Go somewhere</a>
    </div>
  </div>
  <div class="card">
    <h5 class="card-header">Featured -> {{texto}}</h5>
    <div class="card-body">
      <h5 class="card-title">Special title treatment</h5>
      <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
      <a href="#" class="btn btn-primary" v-on:click="letra('A')">Go somewhere A</a>
    </div>
  </div>
  <div class="card">
    <h5 class="card-header">Featured -> {{opcion}}</h5>
    <div class="card-body">
      <h5 class="card-title">Special title treatment</h5>
      <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
      <a href="#" class="btn btn-primary" v-on:click="sumar">Go somewhere</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      opcion: "Opción",
      texto: ""
    }
  },
  methods: {
    sumar: function(){
      this.opcion = 6+4
    },
    letra: function(boton){
      this.texto = "Nueva Opción en Texto " + boton
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
</style>
