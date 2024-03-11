<script setup lang="ts">
</script>

<template>
    <main>
        <section>
            <h1>Chegou o CloudFire bolão de futebol!</h1>
            <p>Desafie seus amigos e se divirta acertando os placares dos jogos do Brasileirão.</p>
            <button>Jogar</button>
        </section>
        <img src="../../public/mainPhoto.png" alt="campo de futebol nos céus">
    </main>
</template>

<style scoped>
main {
    display: flex;
    width: 100%;
    height: 90vh;
}

main section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 50%;
    gap: 15px;
    align-items: center;
    height: 70vh;
}
main img {
    width: 50%;
}

main section h1{
    font-weight: bold;
    font-size: 41px;
    width: 50%;
    text-align: center;
}

main section p{
    font-size: 30px;
    text-align: center;
    width: 50%;
}

main section button{
    background-color: black;
    color: white;
    border-radius: 10px;
    font-size: 26px;
    padding: 8px;
    width: 20%;
}

main section button:hover{
    opacity: 0.8;
}

@media (max-width: 1150px) {
    main section h1{
      font-size: 31px;
      width: 80%;
    }

    main section p{
      font-size: 23px;
      width: 80%;
    }

    main section button{
      font-size: 20px;
      width: 23%;
      padding: 10px;
    }
}

@media (max-width: 700px) {
     main section h1{
      font-size: 25px;
      width: 80%;
    }

    main section p{
      font-size: 20px;
      line-height: 21px;
      width: 80%;
    }

    main section button{
      font-size: 20px;
      width: 30%;
      padding: 10px;
    }
}

@media (max-width: 550px) {
 

    main section button{
      font-size: 20px;
      width: 40%;
      padding: 10px;
    }
}
</style>