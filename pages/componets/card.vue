<template>

        <div class="card">
            <img :src="src" :alt="alternativo">
            <span class="text-center">{{ title }}</span>
        </div>
 
</template>

<script>
    export default {
        props:{
            src:{
                type:String,
            },
            alternativo:{
                type:String,
                default:"imagem freecodecamp"
            },
            title:{
                type:String
            }
            
        },
    }
</script>

<style scoped>

.card{
    width: 412px;
    height: 112px;
}
</style>