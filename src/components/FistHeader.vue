<template>
    <div class="header">
        <img src="../assets/logo.png" alt="">
        <p>borbapa.com.br</p>
    </div>
</template>
  
<script>
export default {
    name: 'FistHeader',
}
</script>
  
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
.header {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px;
    font-size: 15px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    font-style: italic;
}
.header img {
    width: 60px;
    padding: 0 10px;
}

</style>