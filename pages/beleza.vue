<template>
    <div>
        <h1>belezinha</h1>


        <NuxtLink to='/'>
        home
        </NuxtLink>
        <br>
        <br>
        <button v-on:click="asyncData">Buscar emojes</button>
        <div class="lista-class">
            <li v-for=" i in this.lista" :key="i">
                <img v-bind:src=i alt="">
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

        async asyncData() {
            console.log("ois")
            const ip = await this.$axios.$get('https://api.github.com/emojis')
            this.lista = ip
            
        }
    
    },
}
</script>
<style>
    .lista-class{
        display: flex;
        	flex-wrap: wrap;
            list-style:none; 
    }
</style>