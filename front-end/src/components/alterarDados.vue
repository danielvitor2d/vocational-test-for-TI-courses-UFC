<template>
    <div>
        <button id="btn-voltar" @click="goBack">Voltar</button><button id="btn-excluir" @click="delete">Excluir Conta</button>

        <div class="alterarDados">
            <h2>Perfil</h2>
            <form class="formulario">
                <label for="name">Altera nome:</label>
                <input type="text" id="name" name="name" v-model="name" placeholder="Digite seu nome aqui">
                <label for="username">Alterar email:</label>
                <input type="text" id="username" name="username" v-model="username" placeholder="Digite seu email aqui">
                <label for="birthdate">Alterar data de nascimento:</label>
                <input type="date" id="birthdate" name="birthdate" v-model="birthdate">
                <label for="password">Alterar senha:</label>
                <input type="password" id="password" name="password" v-model="password" placeholder="Digite sua senha aqui">
                <label for="password-confirm">Confirmação de senha:</label>
                <input type="password" id="password-confirm" name="password-confirm" v-model="passwordConfirm"
                    placeholder="Confirme sua senha">
            </form>
            <button type="submit" @click.prevent="alterarDados">Alterar Dados</button>
        </div>
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
        alterarDados() {
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

h2 {
    margin-top: -10%;
    text-align: center;
}

.formulario {

    align-content: center;
    margin-top: 10%;

}

.alterarDados {

    width: 30%;
    background-color: #fff;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin: 0 auto;
}

.alterarDados label {
    display: block;
    font-weight: bold;
    margin-bottom: 10px;
    align-items: center;
}

.alterarDados input[type="text"],
.alterarDados input[type="password"],
.alterarDados input[type="date"] {
    width: 100%;
    padding: 8px;
    border: 2px solid #ccc;
    border-radius: 4px;
    margin-bottom: 15px;
}

.alterarDados button[type="submit"] {
    background-color: #007AC2;
    color: #fff;
    border: none;
    border: 3px;
    padding: 8px;
    font-weight: bold;
    cursor: pointer;
    width: 103.5%;
    margin-top: 5%;

}

.alterarDados button[type="submit"]:hover {
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
    width: 7%;
    margin-top: 5%;
    margin-left: 2%;
}

#btn-voltar:hover {
    background-color: #0062a3;
}

#btn-excluir {
    background-color: #D83020;
    color: #fff;
    border: none;
    border: 3px;
    padding: 8px;
    cursor: pointer;
    font-weight: bold;
    width: 7%;
    margin-top: 5%;
    margin-right: 2%;
    float: right;
}

#btn-excluir:hover {
    background-color: #da4c3f;
}</style>