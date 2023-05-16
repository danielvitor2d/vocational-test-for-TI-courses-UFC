<template>
    <div class="popup">
        <header class="borda-cima"></header>
        <h2 class="text">Excluir Conta</h2>
        <p class="text" id="pergunta_exclusao">Tem certaza que deseja excluir sua conta?</p>
        <div class="botoes">
            <button class="botao_cancelar">Cancelar</button><button class="botao_excluir">Excluir</button>
        </div>
    </div>
</template>

<script>


</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');

body {
    font-family: 'inter', sans-serif;
}

.borda-cima {
    background-color: #D83020;
    color: #D83020;
    height: 5px;
    width: 512px;
    position: absolute;
    border-top-left-radius: 6px;
    border-top-right-radius: 6px;



}

.popup {
    background-color: #fff;
    width: 512px;
    height: 256px;
    position: fixed;
    border-top-left-radius: 6px;
    border-top-right-radius: 6px;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    text-align: left;
    box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.75);
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
}

.text {
    margin-left: 6%;
}

#pergunta_exclusao {
    margin-top: 10%;
    margin-left: 6%;
    font-size: 20px;
    font-weight: 700;
    color: #4A4A4A;
}

#h2 {
    font-size: 24px;
}

.botao_cancelar:hover{
    background-color: #cfcfcf;
}

.botao_cancelar {
    background-color: #fff;
    border: 1px solid #007AC2;
    border-radius: 6px;
    width: 125px;
    height: 50px;
    cursor: pointer;
    margin-left: 10%;
    margin-top: 7%;
    font-size: 16px;
    font-weight: 700;
    color: #007AC2;
}
.botao_excluir:hover{
    background-color: #d82f20ce;
}
.botao_excluir {
    background-color: #D83020;
    border: 1px solid #D83020;
    border-radius: 6px;
    width: 100px;
    height: 50px;
    cursor: pointer;
    margin-left: 5%;
    margin-top: 12%;
    font-size: 16px;
    font-weight: 700;
    color: #fff;
}

.botoes{
    margin-left: 40%;
}
</style>