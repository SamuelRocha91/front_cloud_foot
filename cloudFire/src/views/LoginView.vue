<script setup lang="ts">
import { RouterLink } from 'vue-router';

</script>

<template>
    <div id="page-login">
        <div>
            <h1>Login</h1>
            <section class="login-fields">
              <input type="text" placeholder="example@xxxxx.com">
              <input type="text" placeholder="senha">
              <RouterLink id="forgot-Password" to="/login/recovery-password">Esqueceu a senha?</RouterLink>
              <button>Entrar</button>
              <RouterLink id="create-Account" to="/registro">Criar conta</RouterLink>
            </section>
        </div>
    </div>
</template>

<style scoped>
    #page-login {
        display: flex;
        width: 100%;
        height: 100vh;
        justify-content: center;
        align-items: center;
    }

    #page-login div {
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
    #page-login div h1 {
     font-size: 32px;
     font-weight: bold;
    }
 
    .login-fields {
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


    .login-fields button{
        font-size: 20px;
        padding: 10px;
        background-color: black;
        color: white;
        border-radius: 5px;
        transition: background-color 0.3s ease;
    }

      .login-fields button:hover {
        background-color: #333;
    }

    #forgot-Password {
        align-self: end;
    }

    #create-Account {
        align-self: center;
    }

    @media (max-width: 768px) {
        #page-login div {
            width: 80%;
            padding: 20px;
        }

        .login-fields {
            width: 100%;
        }
    }

    @media (max-width: 480px) {
        #page-login div {
            width: 100%;
            padding: 10px;
        }

        .login-fields button {
            width: 100%;
        }
    }
</style>