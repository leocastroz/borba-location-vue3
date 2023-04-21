<template>
  <div>
    <h2>NOSSA LOCALIZAÇÃO</h2>
    <div class="location-map">
        <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d7934.54674433169!2d-49.842111!3d-6.093831!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x92dd5131ba587971%3A0xd2189ff770fbf4b2!2sBORBA!5e0!3m2!1spt-BR!2sbr!4v1682053530948!5m2!1spt-BR!2sbr" width="900" height="300" style="border:0; border-radius: 18px" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"> 
        </iframe>
        <div>
          <p>BORBA SERVIÇOS. Rua 30, Quadra 238, Lote 04, Nova Carajás. Parauapebas-PA, 68515-000.</p>
        </div>
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


div h2 {
  font-family: 'Poppins', sans-serif;
  text-align: center;
}
.location-map {
  margin: 30px auto;
  max-width: 900px;
  font-family: 'Poppins', sans-serif;
  text-align: center;
  background: linear-gradient(261deg, #2a3b89 0%, #0e237e 48%, #2a3b89 100%);
  border-radius: 20px;
  box-shadow: 0 0 8px 0px #8e8e8e;
}

.location-map iframe {
  border-radius: 20px;
}

.location-map div p {
  font-weight: 500;
  font-size: 11px;
  color: #fff;
  padding: 3px 0 6px 0;
}

</style>