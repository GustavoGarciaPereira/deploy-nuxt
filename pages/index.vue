<template>
    
    <div class="div-main">
        <div class="menu-m">
            <h1>gustavo diz olá 
                <span>
                    <img class="rotating" src="https://twemoji.maxcdn.com/2/svg/1f44b.svg" 
                        width="40px" height="40px" alt="">
                </span>
            </h1>

            <NuxtLink class="rotating1" to='/beleza'>
                beleza
            </NuxtLink>
            
            <NuxtLink to='/js-legal'>
                um pouco de javascript
            </NuxtLink>
            <NuxtLink to='/star-wars'>
                Star Wars
            </NuxtLink>
        </div>
            
        
        <div class="img-div">
            <img src="https://i.pinimg.com/originals/3d/f3/eb/3df3eb1714d898fdf69c621ea949b3a3.gif" alt="">
        </div>
        
    </div>


</template>

<style scoped>
.div-main{
    background-color:rgb(21,37,67);
    height: 1000px;
}
.img-div{
    text-align: center;
}
    .menu-m{
    color: azure;
        padding-top: 2rem;
        padding-bottom: 2rem;
        text-align: center;
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
        box-shadow: 10px 10px #81d890;
        /* text-shadow: 3px 2px #558ABB; */
    }

    .rotating {
        transition: transform 0.5s ease-in-out;
    }
    .rotating:hover {
        transform: rotateZ(-100deg);
    }
    h1{
        padding-bottom: 10px;
        text-shadow: 2px 2px #010102;
    }

</style>