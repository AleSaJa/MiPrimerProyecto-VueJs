<template>
    <div>
        <ul>
            <li   li v-for="color in colores" v-bind:key="color">{{color}}</li>
        </ul>
    </div>

    <div>
        <ul   li v-for="color in colores" v-bind:key="color">
            <li>{{color.nameS}} </li>
            <li>{{color.nameI}}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ListaDeObjeto',
    data() {
        return {
            colores: [
                {nameS: 'rojo', nameI: 'red'},
                {nameS: 'verde', nameI: 'green'},
                {nameS: 'amarillo', nameI: 'yellow'},
                {nameS: 'azul', nameI: 'blue'}
            ]
            }
    }
}
</script>

<style>

</style>