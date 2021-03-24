<template>
    <div>
        <figure>
            <img :src="src" width="90px" height="90px" :alt="alternativo">
        </figure>
    </div>
</template>

<script>
    export default {
        props:['src','alternativo'],
        data(){
            
            console.log(this.alternativo)
            this.alternativo = "gustavo"
            return{
                
            }
        }
    }
</script>