<template>
    <div>
        <figure>
            <img :src="src" width="90px" height="90px" :alt="alternativo">
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
            }
        },
    }
</script>