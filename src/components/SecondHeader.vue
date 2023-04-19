<template>
    <div class="header">
       <a href="">Serviços</a>
       <a href="">Empresa</a>
       <a href="">Contato</a>
    </div>
</template>
  
<script>
export default {
    name: 'SecondHeader',
}
</script>
  
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
.header {
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Poppins', sans-serif;
    width: 100%;
    height: 100px;
    background: linear-gradient(261deg, #141c40 0%, #0e237e 48%, #000620 100%);
}

.header a {
    padding: 0 10px;
    color: #fff;
    text-decoration: none;
}

</style>