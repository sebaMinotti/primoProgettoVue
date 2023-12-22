<template>
  
  <HeaderVue />
  <MainVue />
</template>

<script>
import HeaderVue from './components/Header.vue'
import MainVue from './components/Main.vue'
import './reset.css'

export default {
  name: 'App',
  components: {
    HeaderVue ,
    MainVue
  }
}
</script>

<style>
#app {
 
  
}
</style>
