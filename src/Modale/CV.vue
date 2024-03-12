<script>
  export default {
    data() {
      return {
        showModal: false
      };
    },
  }
    

</script>


<template>
  <div>
    <button @click="showModal = true">
      <button id="myBtn">
        <div class="content">
          <img src="../Proj/CV.png" alt="Mon CV" style="width: 100%;">
          <h3>Mon CV</h3>
        </div>                              
      </button>
    </button>
      
    <div v-if="showModal" class="modal">
      <div class="modal-content">
        <span class="close" @click="showModal = false">&times;</span>
        <h4>Réalisation de mon CV</h4>
        <h5>le 16 janvier 2024</h5>
        <p class="title">langages utilisés pour la réalisation:</p>
        <div class="descriptif">
          <div class="langages">            
            <ul>
              <li>HTML pour le balisage du site</li>
              <li>CSS pour la mise en forme</li>
              <li>GitHub pour la sauvegarde et le versionning</li>  
            </ul>
          </div>   
          <div class="Git">      
            <a href="https://github.com/Tintin4522/cv" target="_blank"><img class="lienGit" src="../img/github-logo.png" alt="lien du projet sur linkedin"></a>
          </div> 
        </div>
      </div>
    </div>
  </div>
</template>
   

   
<style scoped>

h3 {
  font-size: 25px;
  text-align: center;
  color: #1da593;
}

h4 {
  font-size: 25px;
  text-align: center;
  color: #1da593;
}

h5 {
  font-size: 18px;
  text-align: center;
  color: #1da593;
}

#myBtn:hover {
  box-shadow: 15px 15px 10px #333;
  cursor: zoom-in;
}

.Git {
  display: flex;
  justify-content: center;
  align-items: center;
}

.lienGit {
  width: 75px;
  height: 75px;
}

.title {
  text-align: center;
  padding-top: 20px;
}

.descriptif {
  text-align: center;
}

.modal {
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0,0,0,0.5);
}
 
.modal-content {
  background-color: #fefefe;
  margin: 15% auto;
  padding: 20px;
  border: 1px solid #888;
  width: 80%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
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