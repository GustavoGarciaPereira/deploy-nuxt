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
            
            <button id="btn_buscar" href="#" v-on:click="asyncData">Buscar emojis</button>
        </div>


        <div class="container">
            <div class="iteins" v-for=" i in this.lista" :key="i[0]">
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
    .container{
        padding: 16px;
        display: flex;
        flex-wrap: wrap;
    }
    .iteins{
        width: 100px;
        height: 100px;
        margin: 24px;
        display: flex;
        align-items: center;
        justify-content: center; 
        padding: 1rem 2rem 2rem 0rem;
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

    #btn_buscar{
        width: 200px;
        height: 40px;
        background-color:rgba(16, 45, 212, 0.514);
        color: rgb(65, 21, 105);
    }

@media (min-width: 427px) {
    .container{
        padding: 13px 10px 10px 80px;
        display: flex;
        flex-wrap: wrap;
    }
    .iteins{
        width: 100px;
        height: 100px;
        margin: 24px;
        display: flex;
        align-items: center;
        justify-content: center; 
        padding: 1rem 2rem 2rem 0rem;
    }
}

</style>