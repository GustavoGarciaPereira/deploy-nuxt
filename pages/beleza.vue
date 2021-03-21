<template>
    <div>
        <title>
            
        </title>
        <h1>belezinha</h1>


        <NuxtLink to='/'>
        home
        </NuxtLink>
        <br>
        <input type="text" value="" placeholder="filtrar emojis">
        <br>
        <button v-on:click="asyncData">Buscar emojis</button>
        <div class="lista-class">
            <li v-for=" i in this.lista" :key="i[0]">
                <figure class="">
                    <img v-bind:src=i[1] v-bind:alt=i[0] width="64px" height="64px">
                    <span @blur="visivel" class='label-menu'> {{ i[0] }} </span>
                    
                </figure>
            </li>
        </div>        
    </div>
</template>
<script>

export default {

    data() {
        return {
            lista:[]
        }
    },
    methods: {
        visivel(){
            console.log("gustavo")
        },

        async asyncData() {
            console.log("ois")
            const nova_lista = []
            const l = await this.$axios.$get('https://api.github.com/emojis')
                
            const lista1 = Object.keys(l)
            lista1.map(function(item){
                nova_lista.push([item,l[item]])
            })

            this.lista = nova_lista
        }
    
    },
}
</script>
<style>
    .lista-class{
        display: flex;
        flex-wrap: wrap;
        list-style:none; 
        flex-direction: row;
        /*flex: 200px;*/
        align-items: center;
        justify-content: space-around;

            
    }

</style>