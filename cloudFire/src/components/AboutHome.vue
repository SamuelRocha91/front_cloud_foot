<script setup lang="ts">
</script>

<template>
        <section class="about">
            <section>
                <h1>CloudFire, o melhor amigo dos apaixonados por futebol!</h1>
                <p>Bem-vindo ao nosso espaço dedicado aos verdadeiros amantes do futebol! Este site nasceu da paixão ardente de um entusiasta do esporte que desejava uma maneira a mais de se divertir com o esporte. Diante da dificuldade de encontrar um site de bolões gratuito, personalizável e funcional, decidi criar minha própria plataforma e compartilhá-la com pessoas que também possuam o mesmo amor pelo jogo.Fiquem à vontade e se divirtam!.</p>
                <button>Comece já!</button>
            </section>
            <img src="../../public/mainPhoto.png" alt="campo de futebol nos céus">
        </section>
</template>

<style scoped>
.about {
    display: flex;
    width: 100%;
    height: 100vh;
}

.about section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 60%;
    gap: 30px;
    align-items: center;
    height: 80vh;
}
.about img {
    width: 40%;
}

.about section h1{
    font-weight: bold;
    font-size: 35px;
    width: 70%;
    text-align: center;
}

.about section p{
    font-size: 27px;
    text-align: center;
    width: 80%;
}

.about section button{
    background-color: black;
    color: white;
    border-radius: 10px;
    font-size: 23px;
    padding: 8px;
    width: 20%;
}

.about section button:hover{
    opacity: 0.8;
}

@media (max-width: 1150px) {
    .about section h1{
      font-size: 31px;
      width: 80%;
    }

    .about section p{
      font-size: 23px;
      width: 80%;
    }

    .about section button{
      font-size: 20px;
      width: 23%;
      padding: 10px;
    }
}

@media (max-width: 700px) {
     .about section h1{
      font-size: 25px;
      width: 80%;
    }

    .about section p{
      font-size: 20px;
      line-height: 21px;
      width: 80%;
    }

    .about section button{
      font-size: 20px;
      width: 30%;
      padding: 10px;
    }
}

@media (max-width: 450px) {
    .about section button{
      font-size: 18px;
      width: 40%;
      padding: 10px;
    }

    .about section h1{
      font-size: 22px;
      width: 95%;
    }

    .about section p{
      font-size: 20px;
      line-height: 21px;
      width: 95%;
    }
}
</style>