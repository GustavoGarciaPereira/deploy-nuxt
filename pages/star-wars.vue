<template>
<div class="container">


    <div class="text-center">
        <NuxtLink to='/'>
            <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
        </NuxtLink>
    </div>

    <h1 class="text-center">planeta do star wars</h1>
    <p>nome planeta : {{ this.dados_planeta.name }}</p>
    <p>diameter planeta : {{ this.dados_planeta.diameter }}</p>
    <p>gravity planeta : {{ this.dados_planeta.gravity }}</p>
    <p>population planeta : {{ this.dados_planeta.population }}</p>
    <p>terrain planeta : {{ this.dados_planeta.terrain }}</p>
    <p>climate planeta : {{ this.dados_planeta.climate }}</p>

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
            const l = await this.$axios.$get('https://swapi.dev/api/planets/1/')
            console.log(l)
            this.dados_planeta = l
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