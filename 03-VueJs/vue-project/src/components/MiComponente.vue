<template>
    <div class="MiComponente">
        <h1>{{libro.titulo}}</h1>
        <h2>{{libro.autor}}</h2>
        <div v-html="libro.datos"></div>
        {{libro.datos}}
        <div>
            {{paginas}}
            <p>{{paginas[0]}}</p>
            <p>{{paginas[1]}}</p>
            <p>{{paginas[2]}}</p>
            <p>{{paginas[3]}}</p>
            <p>{{paginas[4]}}</p>
            <p>{{paginas[5]}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MiComponente',
    data() {
        return{
            libro:{
                titulo: "Tokyo Blues",
                autor: "Haruki Murakami",
                datos: "<h3>Lorem</h3><p>Lorem ipsum dolor</p>"
            },
            paginas: ["pg.1","pg.2","pg.3","pg.4","pg.5","pg.6"]
        }
    },
}
</script>

<style>

</style> 