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
                <p>Ceci est le contenu de la modale.</p>
            </div>
        </div>
    </div>
</template>

<style scoped>

#myBtn:hover {
    box-shadow: 15px 15px 10px #333;
    cursor: zoom-in;
}

h3 {
  font-size: 25px;
  text-align: center;
  color: #1da593;
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

