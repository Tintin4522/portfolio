<script setup>

</script>

<template>
  <h1>Qui suis-je ?</h1>
  <div class="container">
    <img src="../img/Nature.jpg" alt="image nature" style="width: auto;">
    <div class="presMe">
      <div class="textImg">
      <p>
        Bonjour, je m'appelle Tintin4522, j'ai 37 ans et je suis en reconversion professionnelle en tant que Développeur Web. <br>
        Je vais vous présenter ici mes différentes réalisation en HTML, CSS et JavaScript. <br>
        Bonne visite à vous.
      </p>
      </div>
    </div>
  </div>

</template>

<style scoped>

h1 {
  font-size: 50px;
  color: #1da593;
  word-break: break-all;
  text-align: center;
}

p {
  font-size: 25px;
  font-weight: 800;
}

* {
  box-sizing: border-box;
}

.container {
  background-color: #483d3f;
  position: relative;
  display: flex;
  justify-content: center;
  width: 100%;
}

.presMe {
  position: absolute;
  top: 50%;
  width: 50%;
  background-color: aliceblue;
  text-align: center;
  opacity: 3;
}

.textImg {
    position: absolute;
  width: 100%;
  height: 100%;
  color: black;
  font-size: 1.5rem;
  opacity: 1;
}


</style>



