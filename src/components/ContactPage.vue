<script>




</script>

<template>
    <h1>Me contacter</h1>
    <div class="local">
      <div class="name">
        <label for="name">Nom :</label>
        <input type="text" id="name">
      </div>
      <div class="email">
        <label for="email">E-mail :</label>
        <input type="email" id="email">
      </div>
    </div>  
      <div class="message">
        <label for="message">Message :</label>
        <textarea id="message"></textarea>
      </div>      
    
    <button type="submit">Envoyer</button>
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
  color: #1da593;
}

.email label {
  font-size: 20px;
  word-break: break-all;
  text-align: center;
  color: #1da593;
}

.message label {
  font-size: 30px;
  word-break: break-all;
  text-align: center;
  color: #1da593;
}

.local {
  display: grid;
  grid-template-columns: repeat(2, 2fr);
  grid-template-rows: repeat(1, 2fr);
}

.name {
  display: table;
  grid-column: 1/2;
  border: 3px solid #1da593;
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
  border: 3px solid #1da593;
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
  border: 3px solid #1da593;
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
  border: 2px outset #1da593;
}

button {
  margin: 0 auto;
  display: block;
  border: 5px solid #1da593;
  background-color: #f1f1f1;
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
  border: 2px outset #1da593;
  padding: 25px;
  font-size: 25px;
}

</style>