<template>
<div>
<div class="box">

<NuxtLink id="menu" to='/'>
    <img src="https://cdn.onlinewebfonts.com/svg/img_394318.png" width="50px" height="50px" alt="">
</NuxtLink>

</div>

    <div id="main">
        <a href="#primera_materia" class="btn">básico js</a>
        <a href="#segunda_materia" class="btn">react in cdn</a>

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
<p>como podemos usar o react com cdn</p>
<p>primeiramente devemos importar o cdn do react</p>
<p>onde tem todos os códgio e biblioteca que presisamos</p>

<pre style="color:#55cc66;background:#001800;">  <span style="color:#808030; ">&lt;</span>script crossorigin src<span style="color:#808030; ">=</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">https://unpkg.com/react@17/umd/react.development.js</span><span style="color:#800000; ">"</span><span style="color:#808030; ">&gt;</span><span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>script<span style="color:#808030; ">&gt;</span>
  <span style="color:#808030; ">&lt;</span>script crossorigin src<span style="color:#808030; ">=</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">https://unpkg.com/react-dom@17/umd/react-dom.development.js</span><span style="color:#800000; ">"</span><span style="color:#808030; ">&gt;</span><span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>script<span style="color:#808030; ">&gt;</span>
  <span style="color:#808030; ">&lt;</span>script src<span style="color:#808030; ">=</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">https://unpkg.com/babel-standalone@6/babel.min.js</span><span style="color:#800000; ">"</span><span style="color:#808030; ">&gt;</span><span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>script<span style="color:#808030; ">&gt;</span>
</pre>




<pre style="color:#55cc66;background:#001800;">  <span style="color:#508050; font-weight:bold; ">const</span> frontEndFrameworks <span style="color:#808030; ">=</span> <span style="color:#808030; ">[</span>
  <span style="color:#800000; ">'</span><span style="color:#cc5555; ">React</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span>
  <span style="color:#800000; ">'</span><span style="color:#cc5555; ">Angular</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span>
  <span style="color:#800000; ">'</span><span style="color:#cc5555; ">Ember</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span>
  <span style="color:#800000; ">'</span><span style="color:#cc5555; ">Knockout</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span>
  <span style="color:#800000; ">'</span><span style="color:#cc5555; ">Backbone</span><span style="color:#800000; ">'</span><span style="color:#808030; ">,</span>
  <span style="color:#800000; ">'</span><span style="color:#cc5555; ">Vue</span><span style="color:#800000; ">'</span>
<span style="color:#808030; ">]</span><span style="color:#800080; ">;</span>
</pre>


<pre style="color:#55cc66;background:#001800;">  <span style="color:#508050; font-weight:bold; ">function</span> Fun<span style="color:#808030; ">(</span><span style="color:#808030; ">)</span><span style="color:#800080; ">{</span>
    <span style="color:#508050; font-weight:bold; ">const</span> lista <span style="color:#808030; ">=</span> frontEndFrameworks<span style="color:#808030; ">.</span><span style="color:#508050; font-weight:bold; ">map</span><span style="color:#808030; ">(</span><span style="color:#808030; ">(</span>iten<span style="color:#808030; ">,</span>index<span style="color:#808030; ">)</span><span style="color:#808030; ">=</span><span style="color:#808030; ">&gt;</span><span style="color:#800080; ">{</span>
      <span style="color:#508050; font-weight:bold; ">return</span> <span style="color:#808030; ">&lt;</span>li key<span style="color:#808030; ">=</span><span style="color:#800080; ">{</span>index<span style="color:#800080; ">}</span><span style="color:#808030; ">&gt;</span><span style="color:#800080; ">{</span>iten<span style="color:#800080; ">}</span><span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>li<span style="color:#808030; ">&gt;</span>
    <span style="color:#800080; ">}</span><span style="color:#808030; ">)</span>
    <span style="color:#508050; font-weight:bold; ">return</span> <span style="color:#808030; ">(</span>
      <span style="color:#808030; ">&lt;</span>div<span style="color:#808030; ">&gt;</span>
        <span style="color:#808030; ">&lt;</span>h1<span style="color:#808030; ">&gt;</span>FrontEnd Frameworks<span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>h1<span style="color:#808030; ">&gt;</span>
        <span style="color:#808030; ">&lt;</span>ul<span style="color:#808030; ">&gt;</span>
          <span style="color:#808030; ">&lt;</span>h5<span style="color:#808030; ">&gt;</span>FrontEnd Frameworks<span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>h5<span style="color:#808030; ">&gt;</span>
          <span style="color:#800080; ">{</span>lista<span style="color:#800080; ">}</span>
        <span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>ul<span style="color:#808030; ">&gt;</span>
      <span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>div<span style="color:#808030; ">&gt;</span>
    <span style="color:#808030; ">)</span>
  <span style="color:#800080; ">}</span>
</pre>



<pre style="color:#55cc66;background:#001800;">  ReactDOM<span style="color:#808030; ">.</span>render<span style="color:#808030; ">(</span>Fun<span style="color:#808030; ">(</span><span style="color:#808030; ">)</span><span style="color:#808030; ">,</span> document<span style="color:#808030; ">.</span>getElementById<span style="color:#808030; ">(</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">root</span><span style="color:#800000; ">"</span><span style="color:#808030; ">)</span><span style="color:#808030; ">)</span>
</pre>


<pre style="color:#55cc66;background:#001800;">  <span style="color:#808030; ">&lt;</span>div id<span style="color:#808030; ">=</span><span style="color:#800000; ">"</span><span style="color:#cc5555; ">root</span><span style="color:#800000; ">"</span><span style="color:#808030; ">&gt;</span><span style="color:#808030; ">&lt;</span><span style="color:#808030; ">/</span>div<span style="color:#808030; ">&gt;</span>
</pre>


    </div>
</div>
</template>

<style scoped>
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