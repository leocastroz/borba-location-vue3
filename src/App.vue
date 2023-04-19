<template>
  <div>
    <PreLoader v-if="showPreLoader" />
    <div v-if="!showPreLoader" class="texto">
      <FistHeader />
      <SecondHeader />
    </div>
  </div>
</template>

<script>
import FistHeader from './components/FistHeader.vue'
import SecondHeader from './components/SecondHeader.vue'
import PreLoader from './components/PreLoader.vue'

export default {
  name: 'App',
  components: {
    PreLoader,
    FistHeader,
    SecondHeader,
  },
  data() {
    return {
      showPreLoader: true
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