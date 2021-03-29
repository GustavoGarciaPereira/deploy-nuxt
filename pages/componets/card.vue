<template>

        <figure>
            <img :src="src" width="90px" height="90px" :alt="alternativo">
            <div>{{ title }}</div>
        </figure>
 
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


    }
    figure{
        background: #eee;
        padding: 2rem;
        width: 100px;
        align-items: center;
        text-align: center;
        border: 2px solid rgb(199, 189, 189);
        flex-direction: column;

    }
</style>