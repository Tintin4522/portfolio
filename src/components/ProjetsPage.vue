<script setup>




</script>

<template>
    <div class="projets" >
        <h1>Mes projets</h1>

        <h2>Voici une présentation des mes réalisations</h2>
        

        <div class="imgProjets">
            <div class="column">
                
                <button id="myBtn">
                <div class="content">
                    <img src="../Proj/CV.png" alt="Mon CV" style="width: 100%;">
                    <h3>Mon CV</h3>
                </div>                              
                </button>
                
            </div>
        
            <div class="column">
                <div class="content">
                    <img src="../Proj/Cahier.png" alt="Cahier des charges" style="width: 100%;">
                    <h3>Cahier des charges</h3>
                </div>
            </div>
            <div class="column">
                <div class="content">
                    <img src="../Proj/Commentaire.png" alt="espace commentaire" style="width: 100%;">
                    <h3>Espace commentaire dynamique</h3>
                </div>
            </div> 
        </div>
    </div>
</template>

<style scoped>

/* CSS de la page*/
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
    color: #1da593;
}

h2 {
    font-size: 35px;
    word-break: break-all;
    text-align: center;
    color: #1da593;
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
    font-size: 25px;
    text-align: center;
    color: #1da593;
}

.content {
    background-color:#f1f1f1;
    padding: 15px;
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

img:hover {
    box-shadow: 15px 15px 10px #333;
}

/* CSS du modale*/


</style>