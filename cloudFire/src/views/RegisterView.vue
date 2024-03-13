<script setup lang="ts">
import { ref } from 'vue';
import { RouterLink } from 'vue-router';

const state = ref({
    email: "",
    password: "",
    passwordRepetition: "",
})

</script>

<template>
    <div id="page-register">
        <div>
            <h1>Registro</h1>
            <section class="register-fields">
              <input v-model="state.email" type="text" placeholder="Digite seu email">
              <input v-model="state.password" type="password" placeholder="Digite uma senha">
              <input v-model="state.passwordRepetition" type="password" placeholder="Repita a senha">
              <button>Cadastrar</button>
              <RouterLink id="create-Account" to="/login">Já tenho uma conta</RouterLink>
            </section>
        </div>
    </div>
</template>

<style scoped>
    #page-register {
        display: flex;
        width: 100%;
        height: 100vh;
        justify-content: center;
        align-items: center;
    }

    #page-register div {
        display: flex;
        flex-direction: column;
        justify-content: start;
        align-items: center;
        width: 42%;
        gap: 50px;
        padding: 30px;
        height: 60%;
        background-color: #ffffff;
    }
    #page-register div h1 {
     font-size: 32px;
     font-weight: bold;
    }
 
    .register-fields {
        display: flex;
        flex-direction: column;
        width: 80%;
        gap: 5px;
    }

    input {
       font-size: 20px;
        padding: 10px;
        text-align: center;
        border: 1px solid #ccc;
        border-radius: 5px;
        margin-bottom: 10px;
    }


    input::placeholder{
        text-align: center;
    }


    .register-fields button{
        font-size: 20px;
        padding: 10px;
        background-color: black;
        color: white;
        border-radius: 5px;
        transition: background-color 0.3s ease;
    }

      .register-fields button:hover {
        background-color: #333;
    }

    #forgot-Password {
        align-self: end;
    }

    #create-Account {
        align-self: center;
    }

    @media (max-width: 768px) {
        #page-register div {
            width: 80%;
            padding: 20px;
        }

        .register-fields {
            width: 100%;
        }
    }

    @media (max-width: 480px) {
        #page-register div {
            width: 100%;
            padding: 10px;
        }

        .register-fields button {
            width: 100%;
        }
    }
</style>