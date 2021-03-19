<template>
    <div>
        <NuxtLink to='/'>
            home
        </NuxtLink>

        <h1>Primeiro é presiso caminhar para para depois correr!</h1>
        <div>
            <p>eu corri, cai e me machuquei hoje estou aprendendo a ander!</p>
            <p>mas com a espetiencia de ter caido!</p>

        </div>


        <h2>o que aprendi hoje com javascrit</h2>
        <h3>adicionar no array</h3>
        <p>modificar arrays</p>
        <p>para adicionar um elemento no ultimo lugar do array</p>
        <p>temos o metodo push</p>




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


<p>também temos um metodo bem simples para imformar o polocar no</p>
<p>primeira posição metodo unshift</p>



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



<h3>temos ainda os metodos de remoção</h3>
<p>o uso mais basico é não passando nenhum parametro já que estavamos</p>
<p>removando de um array pre existente</p>
<p>primeiro com o metodo pop</p>

<pre style="color:#55cc66;background:#001800;"><span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> 
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span>pop<span style="color:#808030; ">(</span><span style="color:#808030; ">)</span>
<span style="color:#800000; ">'</span><span style="color:#cc5555; ">novo ultomo</span><span style="color:#800000; ">'</span>
<span style="color:#808030; ">&gt;</span> 
</pre>


<p>e o metodo que remove o primeiro</p>
<p>metodo shift</p>

<pre style="color:#55cc66;background:#001800;"><span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> array<span style="color:#808030; ">.</span><span style="color:#508050; font-weight:bold; ">shift</span><span style="color:#808030; ">(</span><span style="color:#808030; ">)</span>
<span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span>
<span style="color:#808030; ">&gt;</span> array
<span style="color:#808030; ">[</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">gu</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span> <span style="color:#800000; ">'</span><span style="color:#cc5555; ">ultimo</span><span style="color:#800000; ">'</span> <span style="color:#808030; ">]</span>
<span style="color:#808030; ">&gt;</span> 
</pre>

</div>
</template>

<style>
    .code{
        padding-left: 50px;
        padding-right: 50px;
    }
</style>