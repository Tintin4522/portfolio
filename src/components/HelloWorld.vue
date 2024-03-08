<script setup>

</script>

<template>
  <div class="greetings">
    <!--<figure><a href="../img/photo.jpg" target="_blank"><img src="../img/photo.jpg" alt="photo candidat"></a></figure>-->
    <div class="navBar">  
      <a href="">Présentation</a>
      <a href="">Mon CV</a>
      <a href="">Cahier des charges</a>
      <a href="">Espace commentaire dynamique</a>
      <a href="">Me contacter</a>
      <input type="image" class="btnUp" src="../img/">
    </div>
  </div>
</template>

<style scoped>
/*button img {
  border-radius: 50%;
  width: 100%;
  height: 100%;
  object-fit: cover;
  box-shadow: 0 0 30px #2c1d27;
}*/

.btnUp {
  width: 50px;
  height: 50px;
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
}

.main {
  margin-top: 255px;
}
</style>
