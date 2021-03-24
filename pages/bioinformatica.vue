<template>
    <div>
        <h1>bioinformatica</h1>
        

        <div id="pergunta">
        <label for="text"> entre com a sequência</label>
        <input type="text" value="ac">
        <a href="#">
            Enter
        </a>
        </div>
        <div id="resposta">
        <label for="text">resposta</label>
        <input type="text">

        </div>

    </div>
</template>
<script>
export default {
    
}
</script>


<style>
    h1{
        display: flex;
        justify-content: center;
    }
    #pergunta,#resposta{
        padding: 23px;
    }


</style>