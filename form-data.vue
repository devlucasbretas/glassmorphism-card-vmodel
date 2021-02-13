<template>
    <div class="container">
        <div class="form">
            <h1>Peça o seu Cartão</h1>
            <input type="text" v-model="nomeCliente" placeholder="Nome que deverá aparecer no cartão">
            <input type="number" step="50.0" v-model="limite" placeholder="Defina o Seu Limite R$">
        </div>
        <div>
            <div class="card">
                <h2>Lubank</h2>
                <div class="chip"></div>
                <p> {{ nomeCliente }} </p>
            </div>
            <p id="limite">Seu Limite R$ {{ limite }} </p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            nomeCliente: "",
            limite: "",
        }
    }
}
</script>

<style scoped>

    @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@1,700&display=swap');   
    @import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Sans&display=swap');

    body {
        padding: 0px;
        width: 100%;
        box-sizing: border-box;
    }

    h1 {
        margin-left: 10px;
    }

    .container {
        z-index: 1;
        position: relative;
        width: 100%;
        
        display: flex;
        
    }

    .form {
        text-align: center;
        padding: 20px;
        width: 350px;
        height: 440px;
        margin: 55px 100px;
        position: relative;
        justify-content: center;
        box-shadow: 20px 20px 50px  rgba(0, 0, 0, 0.5);
        border-radius: 15px;
        background: rgba(255, 255, 255, 0.1);
        overflow: hidden;
        border-top: 1px solid rgba(255, 255, 255, 0.5);
        border-left: 1px solid rgba(255, 255, 255, 0.5);
        backdrop-filter: blur(5px);
    }

    .form h1 {
        font-family: 'Roboto', sans-serif;
        color: rgb(194, 191, 192);
    }

    p#limite {
        color: rgb(207, 207, 207);
        font-size: 15pt;
        font-family: 'IBM Plex Sans', sans-serif;
        margin-top: 40px;
        margin-left: 240px;
        box-shadow: 20px 20px 50px  rgba(0, 0, 0, 0.5);
        border-radius: 15px;
        background: rgba(255, 255, 255, 0.1);
        overflow: hidden;
        border-top: 1px solid rgba(255, 255, 255, 0.5);
        border-left: 1px solid rgba(255, 255, 255, 0.5);
        backdrop-filter: blur(5px);
        width: 370px;
        height: 40px;
        padding: 10px;
    }
        
    

    .form input {
        margin-bottom: 20px;
        height: 30px;
        border: none;
        border-bottom: 2px solid rgb(250, 36, 90);
        background: transparent;
        width: 250px;
        color: thistle;
    }

    .card {
        padding: 30px;
        width: 330px;
        height: 170px;
        margin-top: 180px;
        margin-left: 240px;
        position: relative;
        box-shadow: 20px 20px 50px  rgba(0, 0, 0, 0.5);
        border-radius: 15px;
        background: rgba(255, 255, 255, 0.1);
        overflow: hidden;
        border-top: 1px solid rgba(255, 255, 255, 0.5);
        border-left: 1px solid rgba(255, 255, 255, 0.5);
        backdrop-filter: blur(5px);
    }

    .card h2 {
        margin: 0px 0px;
        font-family: 'Roboto', sans-serif;
        color: rgb(250, 36, 90);
    }

    .chip {
        margin-top: 30px;
        width: 40px;
        height: 30px;
        border-radius: 5px;
        background: linear-gradient(to right, rgba(165, 165, 165, 0.815), rgba(119, 119, 119, 0.726));
    }

    .card p {
        margin-top: 45px;
        font-family: 'IBM Plex Sans', sans-serif;
        text-transform: uppercase;
        color: rgba(255, 248, 248, 0.884);
        font-size: 14pt;
    }
</style>