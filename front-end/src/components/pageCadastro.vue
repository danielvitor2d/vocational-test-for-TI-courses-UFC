<template>
    <div class="page">
      <div class="left">
        <div class="login">
          <h2>Cadastro</h2>
          <form>
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name" v-model="name" placeholder="Digite seu nome aqui">
            <label for="username">Email:</label>
            <input type="text" id="username" name="username" v-model="username" placeholder="Digite seu email aqui">
            <label for="birthdate">Data de nascimento:</label>
            <input type="date" id="birthdate" name="birthdate" v-model="birthdate">
            <label for="password">Senha:</label>
            <input type="password" id="password" name="password" v-model="password" placeholder="Digite sua senha aqui">
            <label for="password-confirm">Confirmação de senha:</label>
            <input type="password" id="password-confirm" name="password-confirm" v-model="passwordConfirm" placeholder="Confirme sua senha">
            <button type="submit" @click.prevent="login">Entrar</button>
          </form>
        </div>
      </div>
      <div class="right"></div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        username: '',
        birthdate: '',
        password: '',
        passwordConfirm: ''
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
    margin-left: 20%;
    margin-top: -10%;
  }
  
  .login label {
    display: block;
    font-weight: bold;
    margin-bottom: 10px;
  }
  
  .login input[type="text"],
  .login input[type="password"],
  .login input[type="date"] {
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
  </style>
  