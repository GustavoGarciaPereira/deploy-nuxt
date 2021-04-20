<template>
<div>
<div class="box">

<NuxtLink id="menu" to='/'>
    <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
</NuxtLink>

</div>

    <div id="main">
        <a href="#primera_materia" class="btn">gustavo</a>
        <a href="#segunda_materia" class="btn">gustavo</a>

        <h1>Primeiro é preciso caminhar para depois correr!</h1>
        <div>
            <p>eu corri, cai e me machuquei hoje estou aprendendo a andar!</p>
            <p>mas com a experiência de ter caído!</p>
        </div>

        <h2 id="primeira_materia">O que aprendi hoje com javascrit</h2>
        <h3>adicionar no array.</h3>
        <p>modificar arrays</p>
        <p>para adicionar um elemento no ultimo lugar do array</p>
        <p>temos o método push</p>

<pre style="color:#55cc66;background:#001800;">
<span style="color:#808030; ">&gt;</span> <span style="color:#508050; font-weight:bold; ">let</span> array <span style="color:#808030; ">=</span> <span style="color:#808030; ">[</span><span style="color:#808030; ">]</span><span style="color:#800080; ">;</span>
<span style="color:#0f4d75; ">undefined</span>
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span>push<span style="color:#808030; ">(</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">"</span><span style="color:#808030; ">)</span>
<span style="color:#778c77; ">1</span>
<span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span>push<span style="color:#808030; ">(</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">novo ultimo</span><span style="color:#800000; ">"</span><span style="color:#808030; ">)</span>
<span style="color:#778c77; ">2</span>
<span style="color:#808030; ">&gt;</span>
</pre>

<p>também temos um método bem simples para informar o colocar no</p>
<p>primeira posição método unshift</p>

<pre style="color:#55cc66;background:#001800;"><span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span><span style="color:#508050; font-weight:bold; ">unshift</span><span style="color:#808030; ">(</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">"</span><span style="color:#808030; ">)</span>
<span style="color:#778c77; ">5</span>
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span><span style="color:#508050; font-weight:bold; ">unshift</span><span style="color:#808030; ">(</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">"</span><span style="color:#808030; ">)</span>
<span style="color:#778c77; ">6</span>
<span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> 
</pre>

<h3>temos ainda os métodos de remoção</h3>
<p>o uso mais básico é não passando nenhum parâmetro já que estávamos</p>
<p>removendo de um array pre existente</p>
<p>primeiro com o método pop</p>

<pre style="color:#55cc66;background:#001800;"><span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> 
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span>pop<span style="color:#808030; ">(</span><span style="color:#808030; ">)</span>
<span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span>
<span style="color:#808030; ">&gt;</span> 
</pre>

<p>e o método que remove o primeiro</p>
<p>método shift</p>

<pre style="color:#55cc66;background:#001800;"><span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span><span style="color:#508050; font-weight:bold; ">shift</span><span style="color:#808030; ">(</span><span style="color:#808030; ">)</span>
<span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span>
<span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> 
</pre>

    </div>

    <div id="main">

        <h2 id="segunda_materia">React in cdn</h2>

<p>vim aqui escrever um texto que eu acho muito legal</p>
<p>como podemos usar o reac com cdn</p>


    </div>
</div>
</template>

<style>
    .code{
        padding-left: 50px;
        padding-right: 50px;
    }
    #main{
        margin: 50px;
        padding-top: 40px;
    }
    #box{
        height: 10em;
        position: relative 
    }
    #menu{
        margin: 0;
        font-size: 30px;
        position: absolute;
        left: 50%;
        margin-right: -50%;
        transform: translate(-50%, -50%);
        padding-bottom: 32px;
        padding-top: 32px;
    }
    a.btn{
            
        margin: 10px;
        font-style:italic;
        text-decoration: none;
        padding: 10px 10px 10px 10px;
        background-color: rgb(140, 184, 63);
        /*color: aliceblue;*/
        color: rgb(51, 99, 5);
        border-radius: 10px;
    
    }
</style>