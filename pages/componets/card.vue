<template>

        <div class="card" style="width='150px'height='150px'">
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

</style>