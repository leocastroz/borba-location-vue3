<template>
  <div>
    <PreLoader v-if="showPreLoader" />
    <div v-if="!showPreLoader" class="texto">
      <FistHeader />
      <SecondHeader />
      <div class="botao-flutuante" @click="showModal = !showModal"> <!-- Adicione o evento de clique aqui -->
        <!-- <a href="https://api.whatsapp.com/send?phone=+5594991511806&text=Olá Borba! Gostaria de alugar um veículo." target="_blank" >Whatsapp</a> -->
        <a>Whatsapp</a>
      </div>
    </div>
    <div v-if="showModal" class="modal">
      <h4 @click="showModal = false">CLIQUE AQUI PARA FECHAR</h4>
      <p>em desevolvimento . . .  </p>
    </div>
  </div>
</template>

<script>
import SecondHeader from './components/SecondHeader.vue'
import FistHeader from './components/FistHeader.vue'
import PreLoader from './components/PreLoader.vue'

export default {
  name: 'App',
  components: {
    SecondHeader,
    FistHeader,
    PreLoader,
  },
  data() {
    return {
      showPreLoader: true,
      showModal: false,
    }
  },
  mounted() {
    setTimeout(() => {
      this.showPreLoader = false
    }, 5000);
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

.modal {
  position: absolute;
  bottom: 20px;
  right: 20px;
  background-color: #128C7E;
  font-family: 'Poppins', sans-serif;
  color: #fff;
  border-radius: 10px;
  min-width: 350px;
  display: grid ;
  align-items: center;
  justify-content: center;
  height: 400px;
  z-index: 999;
}
.modal h4 {
  cursor: pointer;
}


.botao-flutuante {
  font-family: 'Poppins', sans-serif;
  animation: pulo 3s infinite;
  background-color:#25D366;
  text-decoration: none;
  animation-delay: 3s;
  border-radius: 50px;
  padding: 10px 20px;
  position: fixed;
  cursor: pointer;
  z-index: 999;
  bottom: 20px;
  right: 20px;
}

.botao-flutuante a {
  text-decoration: none;
  font-size: 14px;
  color: #fff;
}


/* Definindo a animação */
@keyframes pulo {
  0% {
      transform: translateY(0);
  }
  50% {
      transform: translateY(-8px);
  }
  100% {
      transform: translateY(0);
  }
}


.texto {
  opacity: 0;
  transition: opacity 1s ease-in-out;
  animation: animacaoTexto 5s linear;
  animation-fill-mode: forwards;
}

@keyframes animacaoTexto {
  0% {
    opacity: 0;
  }
  25% {
    opacity: 0.25;
  }
  50% {
    opacity: 0.5;
  }
  75% {
    opacity: 0.75;
  }
  100% {
    opacity: 1;
  }
}
</style>