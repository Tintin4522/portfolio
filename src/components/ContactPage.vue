<script>
import emailjs from '@emailjs/browser'


emailjs.init({
  publicKey: 'N15FlLY8_XtFO7bGj'
})


export default {
  data() {
    return {
      name: '',
      email: '',
      message: '',
    };
  },
  methods: {
    sendEmail(event) {
      event.preventDefault();
      // Je récupère les données saisies dans le formulaire
      const name = this.name.trim();
      const email = this.email.trim();
      const message = this.message.trim();

      // Je vérifie que les champs ne sont pas vides
      if (name === '' || email === '' || message === '') {
        alert('Veuillez remplir tous les champs du formulaire.');
        return;
      }

      // Je rassemble mes données dans une constante
      const formData = {
        name: document.querySelector('#name').value,
        email: document.querySelector('#email').value,
        message: document.querySelector('#message').value,
      };

      // J'envoie le formulaire à EmailJS
      emailjs.sendForm('service_0hyj5t1', 'template_e2sh6qy', document.getElementById('contactForm'), formData)
        .then((response) => {
          console.log('Email envoyé avec succès', response);
          // Réinitialiser le formulaire après l'envoi
          this.name = '';
          this.email = '';
          this.message = '';

          alert('Votre message à bien été envoyé !')
        })
        .catch((error) => {
          console.error('Erreur envoi mail:', error);
        });
    }
  }
};

</script>

<template>
    <form id="contactForm">
      <h1>Me contacter</h1>
      <div class="local">
        <div class="name">
          <label for="name">Nom / Prénom :</label>
          <input type="text" id="name" v-model="name">
        </div>
        <div class="email">
          <label for="email">E-mail :</label>
          <input type="email" id="email" v-model="email">
        </div>
      </div>  
        <div class="message">
          <label for="message">Message :</label>
          <textarea id="message" v-model="message"></textarea>
        </div>      
      
      <button type="submit" @click="sendEmail">ENVOYER</button>
    </form>
</template>

<style scoped>

h1 {
    font-size: 50px;
    word-break: break-all;
    text-align: center;
    color: #1da593;
}

.name label {
  font-size: 20px;
  word-break: break-all;
  text-align: center;
  color: #9297c4;
}

.email label {
  font-size: 20px;
  word-break: break-all;
  text-align: center;
  color: #9297c4;
}

.message label {
  font-size: 30px;
  word-break: break-all;
  text-align: center;
  color: #9297c4;
}

.local {
  display: grid;
  grid-template-columns: repeat(2, 2fr);
  grid-template-rows: repeat(1, 2fr);
}

.name {
  display: table;
  grid-column: 1/2;
  border: 3px solid #9297c4;
  margin: 20px;
  padding: 12px;
  width: 60%;
  height: 30%;
  left: 20%;
  position: relative;
  text-align: center;
  border-radius: 25px;
}

.email {
  display: table;
  grid-column: 2/2;
  border: 3px solid #9297c4;
  margin: 20px;
  padding: 12px;
  width: 60%;
  height: 30%;
  position: relative;
  text-align: center;
  border-radius: 25px;
}

.message {
  display: table;
  border: 3px solid #9297c4;
  margin: 0 auto;
  width: auto;
  top: 25%;
  left: 25%;
  width: 25%;
  text-align: center;
  justify-content: center;
  border-radius: 25px;
}

input {
  width: auto;
  height: auto;
  overflow: visible;
  border-radius: 50px;
  margin: 25px;
  border: 2px outset #9297c4;
  background-color: #F4EBD9;
}

button {
  font-size: 30PX;
  color: #9297c4;
  margin: 0 auto;
  display: block;
  border: 5px solid #9297c4;
  background-color: #F4EBD9;
  top: 25%;
  left: 25%;
  width: 25%;
  text-align: center;
  border-radius: 25px;
  margin-top: 15px;
  height: 75px;
}

button:hover {
  cursor: pointer;
}

textarea {
  width: 1000px;
  height: 250px;
  border-radius: 50px;
  margin: 25px;
  border: 2px outset #9297c4;
  padding: 25px;
  font-size: 25px;
  background-color: #F4EBD9;
}

</style>