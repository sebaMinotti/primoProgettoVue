<template>
  <header>
       
       <h2>{{ title }}</h2>
  </header>
</template>


<script>
  
 export default{
    name:'HeaderVue',
    data(){
          return{
            title:'primo esercizio con vue',
            
          }
    },
    methods:{

    },
    mounted(){

    }
 }
    
</script>


<style scoped>
 header{
    width: 100%;
    height: 100px;
    background-color: #4d4d4d;
    color: white;
    display: flex;align-items: center;
 }
</style>