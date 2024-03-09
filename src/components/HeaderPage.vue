<script setup>

</script>

<template>
  <div class="greetings">
    <div class="navBar">  
      <a href="">Présentation</a>
      <a href="">Mes projets</a>
      <a href="">Me contacter</a>
      <a href="#" ><img class="btnUpPage"  src="../img/home2.png" alt="bouton retour haut page"></a>
    </div>
  </div>
</template>

<style scoped>
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
  color: white;
  background-color: #1da593;
  text-align: center;
}

header, nav {
  color: white;
  background-color: #1da593;
  justify-content: space-between;
}

select, option {
  color: white;
  background-color: #1da593;
  border: white 2px solid;
  margin: 0 0 2rem 0;
}

.navBar  {
  display: flex;
  justify-content: space-around;
  align-items: center;
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
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.navBar a:hover {
  background: hsl(315, 14%, 95%);
  color:#1da593;
  text-decoration: underline;
}

.main {
  margin-top: 255px;
}
</style>
