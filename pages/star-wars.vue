<template>
<div class="container">


    <div id="menu" class="text-center">
        <NuxtLink to='/'>
            <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
        </NuxtLink>
    </div>

<h1 class="text-center">planetas de star wars</h1>
    <div v-for="(item, index) in dados_planeta" :key="index">
        <div class="planetas">
            <div class="card">
                <h2 class="text-center"> {{ item.name }}</h2>
                <p class="text-center">diameter planeta : {{ item.diameter }}</p>
                <p class="text-center">gravity planeta : {{ item.gravity }}</p>
                <p class="text-center">population planeta : {{ item.population }}</p>
                <p class="text-center">terrain planeta : {{ item.terrain }}</p>
                <p class="text-center">climate planeta : {{ item.climate }}</p>
            </div>
        </div>
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
<style scoped>
    h1{
        padding-top: 42px;
        padding-bottom: 12px;  
    }
    #menu{
        padding-top: 42px;
        padding-bottom: 32px;
    }
    .card{
        padding-top: 12px;
        padding-bottom: 12px;
        background-color: rgba(201, 240, 246, 0.479);
        border:solid 2px rgba(201, 240, 246, 0.479) ;
    }
    .planetas{
        padding-bottom: 40px;
    }
    .container{
        padding-top: 30px;
        background-color: rgba(146, 158, 160, 0.479);
    }
</style>