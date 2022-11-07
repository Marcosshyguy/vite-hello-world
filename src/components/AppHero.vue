<script>
    export default{
        data(){
            return {
                immagine:'vue.svg'
            }
        },methods: {
            getImagePath(){
                return new URL(`../assets/${this.immagine}`, import.meta.url).href;
            }
        },
        components:{

        }
    }
</script>

<template>
  <div class="jumbotron">
    <img :src="getImagePath()" alt="">
  </div>

</template>

<style scoped>
    .jumbotron{
        width: 100%;
        height: 30vh;
    }

    .jumbotron img{
        width: 100%;
        height: 100%;
    }
</style>