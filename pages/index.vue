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
            <NuxtLink to='/star-wars'>
                Star Wars
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
        margin: 10px;
        font-style:italic;
        text-decoration: none;
        padding: 10px 10px 10px 10px;
        background-color: rgb(140, 184, 63);
        /*color: aliceblue;*/
        color: rgb(51, 99, 5);
        border-radius: 10px;
    }
    h1{
        padding-left: 60px;
    }
</style>