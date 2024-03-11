<script setup>

const modal = document.getElementById("myModal");
const btn = document.getElementById("myBtn");
const span = document.getElementsByClassName("close")[0];

btn.onclick = function() {
    modal.style.display = "block";
}

span.onclick = function() {
    modal.style.display = "none";
}

window.onclick = function(event) {
    if (event.target === modal) {
        modal.style.display ="none"
    }
}


</script>

<template>

<div id="myModal" class="modal">
    <div>
        <span class="close">&times;</span>
        <p>contenu de la modal</p>
    </div>
</div>

</template>

<style scoped>

.modal-content {
    background-color: #fefefe;
    margin: 15% auto;
    padding: 20px;
    border: 2px solid #888;
    width: 80%;
}

.close {
    color: #aaa;
    float: right;
    font-size: 28px;
    font-weight: bold;
}

.close:hover,
.close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
}


</style>