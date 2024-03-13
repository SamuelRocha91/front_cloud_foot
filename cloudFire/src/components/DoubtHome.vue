<script setup lang="ts">
import { ref } from 'vue';

const state = ref({
  doubtArea: '',
  email: '',
});

const handleClick = () => {
    const regex = /\S+@\S+\.\S+/;
    if (!regex.test(state.value.email)) {
        return window.alert('É necessário digitar um email válido!');
    } else if (state.value.doubtArea.length < 30) {
        return window.alert('Por favor, elabore melhor seu ponto de vista');
    }
    window.alert('Mensagem enviada com sucesso!');
    state.value.doubtArea = '';
    state.value.email = '';
}
</script>

<template>
    <div>
    </div>
    <section id="doubt" >
        <h1>Ouvidoria</h1>
        <textarea name="doubtArea"  v-model="state.doubtArea" cols="30" rows="10" placeholder="Digite aqui sua dúvida ou sugestão"></textarea>
        <input type="text" v-model="state.email" placeholder="email">
        <button @click.prevent="handleClick">Enviar</button>
    </section>
</template>

<style scoped>
#doubt {
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background: linear-gradient(to right, #ffffff 70%, #e0e4e0 70%);
    gap: 10px;
    align-items: center;
}

#doubt textarea {
    height: 70%;
    width: 50.4%;
    background: linear-gradient(to right, #ffffff 87.9%, #e0e4e0 70%);
    padding: 20px;
}

#doubt textarea::placeholder{
    text-align: center;
    line-height: 20; /* Mantém a altura do input */
    font-size: 30px;
}
#doubt h1 {
    font-weight: bold;
    font-size: 31px;
}
#doubt input {
    width: 51.5%;
    text-align: right;
    padding: 10px;
    background: linear-gradient(to right, #ffffff 87.9%, #e0e4e0 70%);
    font-size: 18px;
}

#doubt input::placeholder {
    text-align: end;
    padding: 10px;
    font-size: 18px;
}
#doubt button {
    width: 53.2%;
    background-color: black;
    color: white;
    padding: 10px;
    border-radius: 10px;
    font-size: 23px;
}
@media (max-width: 1230px) {
    #doubt textarea::placeholder{
    font-size: 25px;
}
}

@media (max-width: 1100px) {
    #doubt button {
    width: 54.7%;
}
 #doubt input {
    width: 52.4%;
    background: linear-gradient(to right, #ffffff 87.1%, #e0e4e0 70%);

}
 #doubt textarea {
    background: linear-gradient(to right, #ffffff 87.1%, #e0e4e0 70%);

}
#doubt textarea::placeholder{
    font-size: 20px;
}
}

@media (max-width: 840px) {
    #doubt button {
    width: 55.7%;
}
   #doubt input {
    width: 52.0%;
}

  #doubt textarea::placeholder {
    font-size: 20px;
    line-height: normal;
    text-align: center;
    padding: 40px;
}

@media (max-width: 740px) {
    #doubt button {
    width: 30.3%;
}
   #doubt input {
    width: 81.8%;
    background: linear-gradient(to right, #ffffff 73.4%, #e0e4e0 70%);

}

   #doubt textarea {
    background: linear-gradient(to right, #ffffff 73.4%, #e0e4e0 70%);
    width: 80%;
    height: 50%;
  }
}


@media (max-width: 600px) {
    #doubt button {
    width: 30.0%;
}
   #doubt input {
    width: 82.8%;
        background: linear-gradient(to right, #ffffff 76.1%, #e0e4e0 70%);

}

  #doubt  {
    background: linear-gradient(to right, #ffffff 73.1%, #e0e4e0 70%);

  }
   #doubt textarea {
    background: linear-gradient(to right, #ffffff 76.1%, #e0e4e0 70%);
  }
}

@media (max-width: 450px) {
  #doubt button {
    width: 90.0%;
  }

   #doubt input {
    width: 83.8%;
    background: linear-gradient(to right, #ffffff 73.5%, #e0e4e0 70%);

  }

   #doubt textarea {
    width: 78.8%;
    height: 50%;
    background: linear-gradient(to right, #ffffff 72.5%, #e0e4e0 70%);

  }
}

}
</style>