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
            <li v-for=" i in this.lista" :key="i[0]">
                <figure>
                    <img v-bind:src=i[1] alt="">
                    <figcaption> {{ i[0] }} </figcaption>
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

        async asyncData() {
            console.log("ois")
            const nova_lista = []
            const l = await this.$axios.$get('https://api.github.com/emojis')
                
            //this.lista = ip
            const lista1 = Object.keys(l)
            lista1.map(function(item){
                //console.log(l[item])
                //console.log()
                nova_lista.push([item,l[item]])
                //nova_lista.push()
            })

            this.lista = nova_lista
            //console.log(">>>>>>>>",this.lista)
            //const f = Object.entries(l)
            console.log(typeof(l))

            
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