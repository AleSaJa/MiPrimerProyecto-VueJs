<template>
  <p>{{condicion}}</p>
  <div class="if" v-if="condicion == 'if'">
    <span>Bloque Condicional {{condicion}} con VueJs</span>
  </div>
  <div class="ifelse" v-else-if="condicion == 'if else'">
    <span>Bloque Condicional {{condicion}} con VueJs</span>
  </div>
  <div class="else" v-else>
    <span>Bloque Condicional {{condicion}} con VueJS</span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return{
      condicion: 'else'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.if {
  padding: 1.5rem 3rem;
  display: inline-block;
  background-color: #42b983;
}
.ifelse{
  padding: 1.5rem 3rem;
  display: inline-block;
  background-color: #be99f2;
}
.else{
  padding: 1.5rem 3rem;
  display: inline-block;
  background-color: #f24150;
}
</style>
