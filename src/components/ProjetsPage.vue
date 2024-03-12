<script setup>

import CV from '@/Modale/CV.vue';
import CahierCharges from '@/Modale/CahierCharges.vue';
import ComDynamique from '@/Modale/ComDynamique.vue';

</script>

<template>
    <div class="projets" >
        <h1>Mes projets</h1>

        <h2>Voici une présentation des mes réalisations</h2>
        

        <div class="imgProjets">
            <div class="column">
                <CV />
            </div>
        
            <div class="column">
                <CahierCharges />
            </div>
            <div class="column">
                <ComDynamique />
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
    width: 30%;
    margin: 10px;
}

.projets:after {
    content: "";
    display: table;
    clear: both;
}


.content {
    background-color:#f1f1f1;
    padding: 15px;
    margin-left: 30px;
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