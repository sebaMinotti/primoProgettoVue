<template>
    <div>
     <main>
             <div class="container-fluid box">
                   <h1>{{ titolo }}</h1>
                   <p>{{ paragrafo }}</p>
                   <div class="immagine">
                    <img :src="immagine" alt="">
                   </div>
                   <button @click="change" type="button" class="btn btn-primary">cambia Immagine</button>
             </div>
     </main>
    </div>
</template>

<script>
    export default {
        name:'MainVue',
        data(){
            return{
                    titolo:'primo progetto con vue !',
                    paragrafo:'cambio immagine al click' ,
                    immagine:'https://media-assets.wired.it/photos/618ce6401a74edb062403e85/3:2/w_885,h_590,c_limit/1539681711_avengers-4.jpg',
            }
        },
        methods:{
          change:function(){
                if(this.immagine=='https://media-assets.wired.it/photos/618ce6401a74edb062403e85/3:2/w_885,h_590,c_limit/1539681711_avengers-4.jpg'){
                     this.immagine='https://cdn1.katadata.co.id/media/images/thumb/2019/04/24/2019_04_24-16_14_36_71d2d5d3509bbffcbe64a240a8857fe6_960x640_thumb.jpg'
                } else  {
                     this.immagine='https://media-assets.wired.it/photos/618ce6401a74edb062403e85/3:2/w_885,h_590,c_limit/1539681711_avengers-4.jpg'
                }
          }
        },
        mounted(){

        }
    }
</script>

<style  scoped>
   main{
    width: 100%;
    height: calc(100vh - 100px);
   }
   .box{
    width: 60%;
    height: 35rem;
    background-color: blue;
    margin-top: 10px;display: flex;flex-direction: column;
   }
   .immagine{
    width: 80%;
    height: 60%;
    background-color: red;
   }
   .immagine img{
    width: 100%;height: 100%;
   }
</style>