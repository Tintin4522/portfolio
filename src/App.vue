<script setup>
import HeaderPage from './components/HeaderPage.vue'
import HomePage from './components/HomePage.vue'
import ProjetsPage from './components/ProjetsPage.vue'
import FooterPage from './components/FooterPage.vue'
import ContactPage from './components/ContactPage.vue'
</script>

<template>
  <header>
    <div class="header">
      <HeaderPage />
    </div>
  </header>

  <main>
    <div class="Presentation">
      <HomePage />
    </div>
  
    <div class="Projets">
      <ProjetsPage />
    </div>

    <div class="Contact">
      <ContactPage />
    </div>

  </main>
  
  <footer>
      <FooterPage />
  </footer>
</template>

<style scoped>
* {
  box-sizing: border-box;
  background-color: #f1f1f1;
}

main {
  padding-top: 60px;
  padding-bottom: 60px;
}


</style>
