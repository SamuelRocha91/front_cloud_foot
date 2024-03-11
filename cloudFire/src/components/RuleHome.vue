<script setup lang="ts">
</script>

<template>
        <section id="rule">
            <section >
                <h1>Crie suas próprias regras!</h1>
                <p>Com CloudFire bolão é possível jogar de múltiplas formas:</p>
                <ul>
                    <li>Limite o número de participantes no bolão;</li>
                    <li>Escolha o formato de liga ou copa;</li>
                    <li>Limite quantidade de jogos;</li>
                    <li>Determine regras de pontuação e muito mais!</li>
                </ul>
                <button>Jogar gratuitamente</button>
            </section>
            <img src="../../public/mainPhoto.png" alt="campo de futebol nos céus">
        </section>
</template>

<style scoped>
#rule {
    display: flex;
    width: 100%;
    height: 100vh;
}

#rule section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 60%;
    gap: 30px;
    align-items: center;
    height: 80vh;
}
#rule img {
    width: 40%;
}

#rule section h1{
    font-weight: bold;
    font-size: 35px;
    width: 70%;
    text-align: center;
}

#rule section p{
    font-size: 27px;
    text-align: center;
    width: 80%;
}

#rule section button{
    background-color: black;
    color: white;
    border-radius: 10px;
    font-size: 20px;
    padding: 8px;
    width: 20%;
}

#rule section button:hover{
    opacity: 0.8;
}

#rule section ul {
    font-size: 20px;
    line-height: 23px;
    text-align: start;
    width: 53%;
    list-style: circle;
}
@media (max-width: 1150px) {
    #rule section h1{
      font-size: 31px;
      width: 80%;
    }

    #rule section p{
      font-size: 23px;
      width: 80%;
    }

    #rule section button{
      font-size: 20px;
      width: 24%;
      padding: 10px;
    }
}

@media (max-width: 990px) {
    #rule section ul {
    width: 55%;
}
   #rule section button{
      font-size: 20px;
      width: 26%;
      padding: 10px 15px;
    }
}

@media (max-width: 950px) {

   #rule section button{
      font-size: 16px;
      width: 30%;
      padding: 10px 15px;
    }
}

@media (max-width: 710px) {
     #rule section h1{
      font-size: 25px;
      width: 80%;
    }

    #rule section p{
      font-size: 20px;
      line-height: 21px;
      width: 80%;
    }

    #rule section button{
      font-size: 16px;
      width: 80%;
      padding: 10px 15px;
    }
}

@media (max-width: 450px) {
    #rule section button{
      font-size: 15px;
      width: 80%;
      padding: 10px;
    }

    #rule section h1{
      font-size: 22px;
      width: 95%;
    }

    #rule section p{
      font-size: 20px;
      line-height: 21px;
      width: 95%;
    }
}
</style>