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
main {
  padding-top: 225px;
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


</style>
