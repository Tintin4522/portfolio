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
            <img src="../Proj/Cahier.png" alt="Cahier des charges" style="width: 100%;">
            <h3>Cahier des charges</h3>
          </div>                              
        </button>
      </button>
        
      <div v-if="showModal" class="modal">
        <div class="modal-content">
          <span class="close" @click="showModal = false">&times;</span>
          <h4>Réalisation d'un cahier des charges pour un client</h4>
          <h5>le 22 janvier 2024</h5>
          <p class="title">Technoogies utlisées:</p>
          <div class="descriptif">
            <div class="langages">
              <ul>
                <li> -> Publisher pour la mise en page, création du contenue et conversion en format PDF</li>
                <li> -> Internet pour l'étude de la concurrence</li>  
              </ul>
            </div>
            <div class="details">
              <p>Veuillez cliquer sur l'icône ci-dessous pour télécharger le cahier des charges complet :</p>
              <p class="LienDll">         
              <a href="../Fichiers/Cahier des charges La Socketterie.pdf" download=""><img class="imgDll" src="../img/download-icon.png" alt="lien du projet sur linkedin"></a>
              </p>
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

.imgDll {
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