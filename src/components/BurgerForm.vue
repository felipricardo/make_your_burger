<template>
    <div>
        <p>Compenente de Mensagem</p>
        <div>
            <form id="burger-form">
                <div clss="input-container">
                    <label for="nome">Nome do cliente:</label>
                    <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite o seu nome">
                </div>
                <div clss="input-container">
                    <label for="pao">Escolha o pão:</label>
                    <select name="pao" id="pao" v-model="pao">
                        <option value="pao-simples">Pão simples</option>
                        <option value="pao-gengibre">Pão de gengibre</option>
                        <option value="pao-italiano">Pão italiano</option>
                    </select>
                </div>
                <div class="input-container">
                    <label for="carne">Escolha a carne do seu burger:</label>
                    <select name="carne" id="carne" v-model="carne">
                        <option value="">Selecione o tipo de carne </option>
                        <option value="maminha">Maminha</option>
                    </select>
                </div>
                <div class="input-container">
                    <label for="opcionais-title">Selecione os opcionais</label>
                    <div class="checkbox-container">
                        <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                        <span>Salame</span>
                    </div>
                </div>
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                    <span>Salame</span>
                </div>
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                    <span>Salame</span>
                </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: "BurgerForm"
}
</script>

<style scoped>
    #burger-form {
        max-width:400px;
        margin: 0 auto;
    }

    .inpput-container {
        display: flex;
        flex-direction: column;
        margin-bottom: 20px;
    }

    label {
        font-weight: bold;
        margin-bottom: 15px;
        color: #222;
        padding: 5px 10px;
        border-left: 4px solid #FCBA03;
    }

    input, select {
        padding: 5px 10px;
        width: 300px;
    }

    #opcionais-container {
        flex-direction: row;
        flex-wrap: wrap;
    }

    #opcionais-title {
        width: 100%;
    }

    .checkbox-container {
        display: flex;
        align-items: flex-start;
        width: 50%;
        margin-bottom: 20px;
    }

    

</style>