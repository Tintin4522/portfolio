<script>
export default {
  data() {
    return {
      showModal: false
    }
  }
}
</script>


<template>
    <div>
        <button @click="showModal = true">
            <button id="myBtn">
                <div class="content">
                    <img src="../Proj/Commentaire.png" alt="espace commentaire" style="width: 100%;">
                    <h3>Espace commentaire dynamique</h3>
                </div>                              
            </button>
        </button>
        
        <div v-if="showModal" class="modal">
            <div class="modal-content">
                <span class="close" @click="showModal = false">&times;</span>
                <h4>Réalisation d'un espace commentaire dynamique</h4>
                <h5>le 08 février 2024</h5>
                <p class="title">Langages utilisés pour la réalisation :</p>
                <div class="descriptif">
                    <div class="langages">            
                        <ul>
                            <li> -> HTML pour le balisage du site</li>
                            <li> -> CSS importer depuis internet</li>
                            <li> -> JavaScript pour la dynamisation sur le site</li>
                            <li> -> GitHub pour la sauvegarde et le versionning</li>  
                        </ul>
                    </div>   
                <div class="Git">      
                <a href="https://github.com/Tintin4522/EspaceCommentaire" target="_blank"><img class="lienGit" src="../img/github-logo.png" alt="lien du projet sur linkedin"></a>
          </div> 
        </div>
      </div>
        </div>
    </div>
</template>

<style scoped>
* {
  font-family: Ojuju;
  font-weight: 600;
}

h3 {
  font-size: 25px;
  text-align: center;
  color: #1da593;
}

h4 {
  font-size: 25px;
  text-align: center;
  color: #f1f1f1;
}

h5 {
  font-size: 20px;
  text-align: center;
  color: #f1f1f1;
}

ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  margin-bottom: 50px;
}

#myBtn:hover {
  box-shadow: 15px 15px 10px #f4ebd9;
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
  color: white;
}

.descriptif {
  text-align: center;
  color: white;
}

.modal {
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgba(255, 255, 255, 0.25);
}
 
.modal-content {
  background-color: #77685D;
  margin: 15% auto;
  padding: 20px;
  border: 3px solid #9297c4;
  width: 80%;
}
 
.close {
  background-color: #1da593;
  color: #f4ebd9;
  float: right;
  font-size: 28px;
  font-weight: bold;
  padding-left: 5px;
  padding-right: 5px;
  margin-top: 5px;
  border-radius: 10px;
  border: 3px solid #f4ebd9;
}
 
.close:hover,
.close:focus {
  color: #483d3f;
  text-decoration: none;
  cursor: pointer;
}
  

</style>

