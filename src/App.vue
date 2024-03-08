<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
        <div class="wrapper">
      <HelloWorld msg="You did it!!!!!!!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>

  <footer>
      <div>
      <a href="https://www.linkedin.com/in/kevin-pierre-776b742a9" target="_blank"><img src="./img/linkedin-logo.png" alt="lien linkedin"></a>
      <a href="https://github.com/Tintin4522" target="_blank"><img src="./img/github-logo.png" alt="lien github"></a>
      <p>dernière mise à jour 08 mars 2024</p>
      </div>
  </footer>


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

footer {
    background-color: #1da593;
    color: white;
    text-align: center;
}

footer img {
    width: 50px;
    height: 50px;
}

footer div {
    align-items: center;
}

footer div a:hover{
    opacity: 0.5;
}


/*header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}*/
</style>
