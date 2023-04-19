<template>
    <div class="preloader">
      <img src="../assets/name_borba.png" alt="">
    </div>
  </template>
  
  <script>
  export default {
    name: 'PreLoader',
  }
  </script>
  
<style scoped>
.preloader {
    background-color: rgb(255, 255, 255);
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100vw;
    height: 100vh;
}

img {
    animation: pulso 1s infinite;
}
  
.preloader img {
    width: 250px;
}
  
@keyframes pulso {
    0% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.2);
    }
    100% {
        transform: scale(1);
    }
}
  
</style>