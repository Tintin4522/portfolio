<script setup>

</script>

<template>
  <div class="greetings">
    <figure><a href="../img/photo.jpg" target="_blank"><img src="../img/photo.jpg" alt="photo candidat"></a></figure>
    <a href="">présentation</a>
    <select name="Creations" id="Create">
      <option value="">Mes créations</option>
      <option value="Mon CV">Mon cv</option>
      <option value="Cahier des charges">Cahier des charges</option>
      <option value="Dynamiser un espace commentaire">Dynamiser un espace commentaire</option>
    </select>
    <a href="">contact</a>
  </div>
</template>

<style scoped>
header img {
    border-radius: 50%;
    width: 100%;
    height: 100%;
    object-fit: cover;
    box-shadow: 0 0 30px #2c1d27;
}


figure {
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


/*h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}*/
</style>
