<template>
    <div class="card-primary">
      <div class="description">
        <h1>HISTÓRIA DA BORBA</h1>
        <p>
          Na data de 27/09/2011 era criada na cidade de Parauapebas no Sudeste do Pará a Empresa C F de Borba Serviços ME, a “BORBA LOCAÇÕES” que após algumas alterações em seu contrato social veio a responder pelo nome fantasia BORBA, o que engloba transporte, locações, turismo e serviços.A Empresa tem como prioridade o respeito ao ser humano, seja ele seu colaborador, cliente, e ou parceiro. Temos como meta a organização e a pontualidade, além da excelência no atendimento ao cliente, que é visto como principal responsável pela sustentabilidade da Empresa.
        </p>
      </div>
      <div class="logo-type">
        <img src="https://scontent.fcks1-1.fna.fbcdn.net/v/t1.18169-9/1743505_610043312376692_722962055_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=174925&_nc_eui2=AeEZHP-0dpk9EM1SNDUnaIr7_eRXSjU9oRX95FdKNT2hFQgDsgr_YijTNoNU4Zt2HsIvO_GUJqp6-TQpm4nLedyW&_nc_ohc=5x-FpeLXbRgAX8byYmN&_nc_ht=scontent.fcks1-1.fna&oh=00_AfCcjQki6o6LZq001vaenCf3FBKUfcdAM6NtLgxPWgKw0g&oe=6469855F" alt="logo">
      </div>
    </div>
</template>

<script lang="ts">
export default {
    data () {
        

        return {}
    }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
.card-primary {
  display: flex;
  align-items: center;
  font-family: 'Poppins', sans-serif;
  border-radius: 20px ;
  padding: 30px;
  margin: 30px auto;
  max-width: 900px;
  background: linear-gradient(261deg, #2a3b89 0%, #0e237e 48%, #2a3b89 100%);
}

.card-primary h1 {
  font-size: 25px;
  color: #fff;
}

.card-primary p {
  color: #c2c2c2;
  font-size: 13px;
  text-align: justify;
  padding: 10px 20px 20px 0;
}

.card-primary .logo-type {
  padding: 20px;
}

.card-primary img {
  border-radius: 100%;
  width: 140px;
}
</style>