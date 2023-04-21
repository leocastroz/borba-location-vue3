<template>
    <div class="container-flex">
        <div class="footer">
            <div class="container-footer">
                <div class="logo-type">
                    <img src="https://scontent.fcks1-1.fna.fbcdn.net/v/t1.18169-9/1743505_610043312376692_722962055_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=174925&_nc_eui2=AeEZHP-0dpk9EM1SNDUnaIr7_eRXSjU9oRX95FdKNT2hFQgDsgr_YijTNoNU4Zt2HsIvO_GUJqp6-TQpm4nLedyW&_nc_ohc=5x-FpeLXbRgAX8byYmN&_nc_ht=scontent.fcks1-1.fna&oh=00_AfCcjQki6o6LZq001vaenCf3FBKUfcdAM6NtLgxPWgKw0g&oe=6469855F" alt="logo">
                </div>
                <div class="description">
                   <div>
                        © Todos os Diretos Reservados - BORBA LOCAÇÕES
                        Feito por Leonardo Castro
                   </div>
                   <div class="social-links">
                        <span class="material-symbols-outlined">
                            group
                        </span>
                        <span class="material-symbols-outlined">
                            rocket_launch
                        </span>
                   </div>
                </div>
            </div>
            <div class="bandeiras">
                <p>NOSSAS BANDEIRAS</p>
                <div>
                    <img width="40px" src="https://static.vecteezy.com/system/resources/previews/020/975/567/original/visa-logo-visa-icon-transparent-free-png.png" alt="">
                    <img width="40px" src="https://w7.pngwing.com/pngs/92/785/png-transparent-mastercard-logo-mastercard-credit-card-payment-visa-nyse-ma-mastercard-logo-text-logo-sign.png" alt="">
                    <img width="60px" src="https://st.recargapay.com/public/av-a/img/lp_pix/LP_Pix_logo_branco.png" alt="">
                    
                </div>
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

.container-flex {
    background-color: #141414;
    padding: 50px 0;
}

.footer {
    background-color: #141414;
    font-family: 'Poppins', sans-serif;
    display: flex;
    margin: 0 auto;
    max-width: 1200px;
    align-items: center;
    justify-content: space-between;
    padding: 0 50px;
}

.container-footer {
    display: flex;
    align-items: center;
    
}

.container-footer .logo-type img {
    width: 150px;
    padding: 20px;
    border-radius: 100%;
}

.container-footer .description {
    max-width: 400px ;
    font-size: 15px;
    color: #fff;
    font-weight: 500;
}
.container-footer .description .social-links span {
    color: #a3a3a3;
    font-size: 18px;
    margin-top: 10px;
    padding: 10px 10px 10px 0;
}

.footer .bandeiras {
    color: #fff;
}

.footer .bandeiras p {
    font-size: 12px;
}

</style>