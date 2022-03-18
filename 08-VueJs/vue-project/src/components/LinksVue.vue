<template>
  <li class="nav-item active">
          <a class="nav-link" v-bind:href="navBarLinks.url">{{navBarLinks.link}}</a>
    </li>
</template>

<script>
export default {
    name: 'LinksVue',
    props: {
        navBarLinks: Object
    }
}
</script>

<style>

</style>