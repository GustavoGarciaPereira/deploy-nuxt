<template>
    <div>
        <figure>
            <img :src="src" width="90px" height="90px" :alt="alternativo">
            <div>{{ title }}</div>
        </figure>
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
    figure{
        display: flex;
flex-direction: column;
    }
</style>