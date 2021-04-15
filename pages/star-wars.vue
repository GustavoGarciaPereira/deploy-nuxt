<template>
<div>
<div class="box">

<NuxtLink id="menu" to='/'>
    <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
</NuxtLink>
</div>
    <div id="main">
        <div>
            
            <p>nome planeta {{ this.nome }}</p>
                
            
            
            
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
            nome:"",
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
            this.nome = l.name

            //this.lista = l
        },

    }
}
</script>
<style>
    .code{
        padding-left: 50px;
        padding-right: 50px;
    }
    #main{
        margin: 50px;
        padding-top: 10px;
    }
    #box{
        height: 10em;
        position: relative 
    }
    #menu{
        margin: 0;
        font-size: 30px;
        position: absolute;
        left: 50%;
        margin-right: -50%;
        transform: translate(-50%, -50%) 
    }
</style>