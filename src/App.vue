<script>
import AppHero from './components/AppHero.vue';
    export default{
        data(){
            return {
                newElement : "La mia prima app con Vite!"

            }
        },methods: {

        },
        components:{
            AppHero
        }
    }
</script>

<template>
  <h1>{{newElement}}</h1>
    <AppHero/>
</template>

<style scoped>
h1{
    text-align: center;
    color: red;
}
</style>
