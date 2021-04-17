<template>
<div class="container">


    <div class="text-center">
        <NuxtLink to='/'>
            <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
        </NuxtLink>
    </div>


    <div v-for="(item, index) in dados_planeta" :key="index">
        
        <h1 class="text-center">planeta do star wars {{ item.name }}</h1>
        <p>nome planeta : {{ item.name }}</p>
        <p>diameter planeta : {{ item.diameter }}</p>
        <p>gravity planeta : {{ item.gravity }}</p>
        <p>population planeta : {{ item.population }}</p>
        <p>terrain planeta : {{ item.terrain }}</p>
        <p>climate planeta : {{ item.climate }}</p>


    </div>


</div>
</template>
<script>
export default {
    components:{},
    data() {
     
        return {
            //lista:[],
            dados_planeta:[]
            //visivel:false 
        }
    },
    created(){
        this.getWeatherData()
    },
    methods:{
        async getWeatherData() {
            const l = await this.$axios.$get('https://swapi.dev/api/planets/')
            console.log(l.results)
            this.dados_planeta = l.results
            //this.lista = l
        },

    }
}
</script>
<style>
    .container{
        padding-top: 30px;
    }
</style>