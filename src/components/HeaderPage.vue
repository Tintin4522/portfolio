<script setup>

</script>

<template>
  <div class="greetings">
    <div class="navBar">  
      <a href="#">ACCUEIL</a>
      <a href="">MES PROJETS</a>
      <a href="">ME CONTACTER</a>
      <a href="#" ><img class="btnUpPage"  src="../img/home2.png" alt="bouton retour haut page"></a>
    </div>
  </div>
</template>

<style scoped>
@font-face {
  font-family: Ojuju;
  src: url(../Police/Ojuju-VariableFont_wght.ttf);
  font-weight: normal;
}

* {
  font-family: Ojuju;
}

.btnUpPage {
  height: 40px;
  width: 40 px;
}

figure {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 150px;
  height: 150px;
  text-align: center;
  padding-top: 25px;
}

figure a:hover {
  cursor: zoom-in;
}

header {
  color: #483d3f;
  background-color: #1da593;
  text-align: center;
}

.navBar  {
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-weight: 800;
}

.greetings {
  overflow: hidden;
  background-color: #1da593;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1;
}

.greetings a {
  float: left;
  display: block;
  color: #483d3f;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.navBar a:hover {
  background: #483d3f;
  color:#f4ebd9;
  text-decoration: underline;
}

.main {
  margin-top: 255px;
}
</style>
