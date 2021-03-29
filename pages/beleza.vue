<template>
    <div>

        <h1>belezinha</h1>

        <div id="menu-beleza">
            <img src="https://s3.amazonaws.com/freecodecamp/camper-image-placeholder.png" 
            width="50px"
            height="50px"
            alt="">                
            <NuxtLink to='/'>
                <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
            </NuxtLink>
            <input type="text" value="" placeholder="filtrar emojis">
            <button v-on:click="asyncData">Buscar emojis</button>
        </div>


        <div class="lista-class">
            <div class="lista" v-for=" i in this.lista" :key="i[0]">
                <card :src="i[1]"
                :alternativo="i[0]"
                :title="i[0]"/>
                <!--
                <figure class="">
                    <img @mouseover="contro_visivel(i[0],$event)"  v-bind:src=i[1] v-bind:alt=i[0] width="64px" height="64px">
                    <span :id='i[0].replaceAll("_","__")' style="display: none;"> {{ i[0] }}</span>
                </figure>
                -->
            </div>
        </div>        
    </div>
</template>
<script>

import card from './componets/card'

export default {

    components:{card},
    data() {
     
        return {
            lista:[],
            visivel:false 
        }
    },
    methods: {
        contro_visivel(event,oi){
            //console.log(this.$el.querySelector('#3rd__place__medal'))
            this.visivel = !this.visivel
        },

        async asyncData() {
            console.log("ois")
            const nova_lista = []
            const l = await this.$axios.$get('https://api.github.com/emojis')
                
            const lista1 = Object.keys(l)
            lista1.map(function(item){
                nova_lista.push([item,l[item]])
            })
            console.log(nova_lista)
            this.lista = nova_lista
        }
    },
}
</script>
<style scoped>

    .lista-class{
        display: flex;
        flex-wrap: wrap;

    }
    #menu-beleza{
    display: flex;


    }
    #menu-beleza{
        background: #eee;
        padding: 2rem;
        align-items: center;
        text-align: center;
        border: 2px solid rgb(199, 189, 189);
        flex-direction: column;

    }

</style>