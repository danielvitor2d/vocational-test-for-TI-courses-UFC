<template>
  <div class="page">
    <div class="left">
      <button id="btn-voltar" @click="goBack">Voltar</button>
      <div class="login">
        <h2>Entre com usa conta</h2>
        <form>
          <label for="username">Email:</label>
          <input type="text" id="username" name="username" v-model="username" placeholder="Digite seu email aqui">
          <label for="password">Senha:</label>
          <input type="password" id="password" name="password" v-model="password" placeholder="Digite sua senha aqui">
          <button type="submit" @click.prevent="login">Entrar</button>
        </form>
        <h5 id="opcao-cadastro">Caso ainda não tenha a conta:</h5>
        <button id="bnt-opcao-cadastro">Cadastro</button>
      </div>
    </div>
    <div class="right"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: ''
    };
  },
  methods: {
    login() {
      // Lógica de autenticação aqui
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');
body {
  font-family: 'inter', sans-serif;
}
h2{
  text-align: center;
  margin-bottom: 11%;
  margin-right: 13.8%;
}
.page {
  display: flex;
  height: 100vh;
}

.left {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
}

.right {
  flex: 1;
  background-image: url('C:\Users\gabri\OneDrive\Documentos\GitHub\vocational-test-for-TI-courses-UFC\front-end/imagem.jpg');
  background-size: cover;
  background-position: center;
  background-color: #fff;
  margin-top: -10%;
}

.login {
  width: 70%;
  margin: 80px;
  top: 0%;
  background-color: #fff;
  padding: 5%;
  border-radius: 0px;
  margin-left: 6%;
  margin-top: -10%;
}

.login label {
  display: block;
  font-weight: bold;
  margin-bottom: 10px;
}

.login input[type="text"],
.login input[type="password"] {
  width: 80%;
  padding: 8px;
  border: 2px solid #ccc;
  border-radius: 4px;
  margin-bottom: 15px;
}

.login button[type="submit"] {
  background-color: #007AC2;
  color: #fff;
  border: none;
  border: 3px;
  padding: 8px;
  font-weight: bold;
  cursor: pointer;
  width: 83.7%;
  margin-top: 15px;
}

.login button[type="submit"]:hover {
  background-color: #0062a3;
}
#btn-voltar {
background-color: #007AC2;
color: #fff;
border: none;
border: 3px;
padding: 8px;
cursor: pointer;
font-weight: bold;
width: 15%;
margin-top: -80%;
margin-left: 2%;
}
#btn-voltar:hover {
background-color: #0062a3;
}
#opcao-cadastro{
  text-align: center;
  margin-left: -17%;
  font-weight: lighter;
  color: rgb(98, 98, 98);
}
#bnt-opcao-cadastro{
  background-color: #fff;
  color: #0062a3;
  border-color: #007AC2;
  border: 10px;
  padding: 8px;
  font-weight: bold;
  cursor: pointer;
  width: 83.7%;


}

</style>
