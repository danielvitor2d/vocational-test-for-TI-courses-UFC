<template>
    <div>
        <header class="Barra">
            <button class="bnt-home">
                <img src="src/assets/logoUfc.png" alt="Imagem da logo da UFC" class="btn-home-image">
            </button>
        </header>

        <body>

        </body>

    </div>
</template>

<script>

</script>

<style>
.Barra {
    background-color: #007AC2;
    color: #007AC2;
    height: 78px;
    width: 100%;
    position: fixed;
    margin-left: -1%;
    margin-right: -2%;
}


.bnt-home {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 9%;
    background-color: #007bc200;
    cursor: pointer;
    border: none;
}

.btn-home-image {
    height: 73px;
    width: 185px;
}
</style>