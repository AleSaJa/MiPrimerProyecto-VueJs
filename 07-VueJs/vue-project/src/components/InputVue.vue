<template>
    <div class="input-group mb-3">
        <h5>{{entradaDeTexto1}}</h5>
        <div class="input-group-prepend">
            <button class="btn btn-outline-secondary" type="button" v-on:click="entradaDeTexto1 = 'Nuevo Texto desde un Boton'">Button</button>
        </div>
        <input type="text" class="form-control" placeholder="" aria-label="" aria-describedby="basic-addon1" v-bind:value="entradaDeTexto1">
    </div>

    <div class="input-group mb-3">
        <h5>{{entradaDeTexto2}}</h5>
        <div class="input-group-prepend">
            <button class="btn btn-outline-secondary" type="button" v-on:click="entradaDeTexto2 = 'Nuevo Texto desde un Boton'">Button</button>
        </div>
        <input type="text" class="form-control" placeholder="" aria-label="" aria-describedby="basic-addon1" v-model="entradaDeTexto2">
    </div>
</template>

<script>
export default {
    name: 'InputVue',
    data(){
        return{
            entradaDeTexto1: 'Texto One Way Bind',
            entradaDeTexto2: 'Texto Two Way Bind'
        }
    }
}
</script>

<style>

</style>