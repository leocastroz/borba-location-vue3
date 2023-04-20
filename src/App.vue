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
      <div class="header-whatsapp">
        <h4>WhatsApp</h4>
        <span @click="showModal = false" class="material-symbols-outlined">
          cancel
        </span>

      </div>
      <div class="side-item">
        <span class="material-symbols-outlined">
          supervisor_account
        </span>
        <p>Pessoas disponíveis</p>
      </div>
      <div class="section-message">
        <div class="image">
          <img width="70" src="https://scontent.fcks1-1.fna.fbcdn.net/v/t1.18169-9/20292794_1081665721964995_7255709146275695161_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=174925&_nc_eui2=AeFVSvsUY9vXOYGoDroPIhctZml21c-rDbFmaXbVz6sNscXfvoMm66iD6yPwd64UVniINPuohwV2CvjukDltECnz&_nc_ohc=fo6iLfzI-YkAX_vfDj8&_nc_ht=scontent.fcks1-1.fna&oh=00_AfA-D5pWtjZPauEk3kXiexcvZ41sBu9G-yRPnDQcL4K3SA&oe=646828E8" alt="">
        </div>
        <div class="message-client">
          <h4>Eliane BORBA</h4>
          <div>
            <span class="material-symbols-outlined">
            done_all
            </span> 
            Olá, vamos conversar ?
          </div>
        </div>
        <div class="arrow">
          <span class="material-symbols-outlined">
            arrow_right
          </span>
        </div>
      </div>

      <div class="section-message">
        <div class="image">
          <img width="70" src="https://scontent.fcks1-1.fna.fbcdn.net/v/t39.30808-6/315898400_2746200162178201_7850748684266171480_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=730e14&_nc_eui2=AeFX0EJo0PhVn06vLkm_cCRamIDkMTggKpCYgOQxOCAqkL7w6sw3wxZ1t5rzEKBXkGVjhhmaBofDZ8cUgx2blXdP&_nc_ohc=Ulu6tS4wmhsAX-5YmjG&_nc_ht=scontent.fcks1-1.fna&oh=00_AfADpfTJq_0fSIohZuxaE-qo_kROB_k8GhMj5F1SoRxpVA&oe=6445BA58" alt="">
        </div>
        <div class="message-client">
          <h4 >Cleiton BORBA</h4>
          <div>
            <span class="material-symbols-outlined">
            done_all
            </span> 
            Olá, vamos conversar ?
          </div>
        </div>
        <div class="arrow">
          <span class="material-symbols-outlined">
            arrow_right
          </span>
        </div>
      </div>

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

.header-whatsapp {
  max-width: 100%;
  height: 70px;
  background-color: #128C7E;
  border-radius: 10px 10px 0 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 15px;
  
}

.header-whatsapp h4 {
  font-weight: 300;
}

.header-whatsapp span {
  cursor: pointer;
}

.side-item {
  display: flex;
  align-items: center;
  justify-content: start;
  gap: 10px;
  padding: 10px 10px;
  height: 40px;
  font-size: 12px;
  max-width: 100%;
  background-color: #128C7E;
  color: #85cdc4;
}

.section-message {
  display: flex;
  color: #000;
  justify-content: space-between;
  border-bottom: 1px solid #a2a1a162;
  align-items: center;
  padding: 15px 5px 0 20px;
}

.section-message .arrow {
  padding: 0 10px;
  cursor: pointer;
} 

.section-message .arrow span {
  color: #a2a1a1;
  font-size: 25px;
  border-radius: 100px;
}

.section-message div img {
  border-radius: 100%;
}



.message-client h4 {
  font-weight: 400;
}
.message-client div {
  
  color: #a2a1a1;
  font-size: 14px;  
  display: flex;

}

.message-client div span {
  color:#34B7F1;
}

.modal {
  position: absolute;
  bottom: 20px;
  right: 20px;
  background-color: #fff;
  box-shadow: 0 0 5px 1px #c2c2c2;
  font-family: 'Poppins', sans-serif;
  color: #fff;
  border-radius: 10px;
  min-width: 350px;
  
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