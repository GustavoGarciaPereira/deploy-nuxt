<template>
    
    <div id="box1">
        <title>home</title>
        <div id="menu1">

            <h1>gustavo diz olá 👋</h1>
            <NuxtLink to='/beleza'>
                beleza
            </NuxtLink>
            
            <NuxtLink to='/js-legal'>
                um pouco de javascript
            </NuxtLink>
            
            <!-- 
                <NuxtLink to='/bioinformatica'>
                    Bioinformarica
                </NuxtLink>
            -->
        </div>
    </div>


</template>

<style scoped>
    #box1{
        height: 10em;
        position: relative 
    }
    
    #menu1{
        margin: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        margin-right: -50%;
        transform: translate(-50%, -50%) 
    }
    a{
        margin: 40px;
        font-style:italic;
        text-decoration: none;
        padding: 5px 4px 4px 5px;
        background-color: darkolivegreen;
        color: aliceblue;
        border-radius: 20px;
    }
    h1{
        padding-left: 60px;
    }
</style>