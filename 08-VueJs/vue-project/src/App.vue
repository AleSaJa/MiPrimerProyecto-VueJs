<template>

  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <LinksVue v-for="item in linksNav" v-bind:navBarLinks="item" v-bind:key="item" />
        
      </ul>
      <SearchVue/>
    </div>
  </nav>

  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SearchVue from './components/SearchVue.vue'
import LinksVue from './components/LinksVue.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    SearchVue,
    LinksVue
  },
  data(){
    return{
      linksNav: [
        {link:'Home',url:'./Home'},
        {link:'Link',url:'./Link'},
        {link:'Dropdown',url:'./Dropdown'},
        {link:'Disabled',url:'./Disabled'}
        ]
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
}
</style>
