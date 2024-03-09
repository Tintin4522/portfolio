<script setup>

</script>

<template>
    <div class="projets" >
        <h1>Mes projets</h1>

        <h2>Portfolio</h2>
        <p>Voici une présentation des mes réalisations</p>

        <div class="imgProjets">
            <div class="column">
                <img src="../Proj/CV.png" alt="Mon CV" style="width: 100%;">
                <h3>Mon CV</h3>
            </div>
        
            <div class="column">
                <img src="../Proj/Cahier.png" alt="Cahier des charges" style="width: 100%;">
                <h3>Cahier des charges</h3>
            </div>
        </div>
        <div class="imgProjets">
            <div class="column">
                <img src="../Proj/Commentaire.png" alt="espace commentaire" style="width: 100%;">
                <h3>Espace commentaire dynamique</h3>
            </div>
        </div> 
    </div>
</template>

<style scoped>
* {
    box-sizing: border-box;
}

.projets {
    background-color: #f1f1f1;
    max-width: 1520px;
    margin: auto;
}

h1 {
    font-size: 50px;
    word-break: break-all;
    text-align: center;
}

img > .column {
    padding: 25px;
}

.column {
    float: left;
    width: 33%;
}

.projets:after {
    content: "";
    display: table;
    clear: both;
}

h3 {
    text-align: center;
}

@media screen and (max-width: 600px) {
    .column {
        width: 100%;
    }
}

@media screen and (max-width: 900px) {
    .column {
        width: 50%;
    }
}

</style>