<template>
    <div class="container">
        <div class="dados">
            <div class="card">
                <h1>12</h1>
                <div class="description">
                    12 anos de mercado e inúmeros
                    contratos fechados
                </div>
            </div>

            <div class="card">
                <h1>7</h1>
                <div class="description">
                    Lorem Episum gray
                    spray master
                    livinu
                </div>
            </div>

            <div class="card">
                <h1>103</h1>
                <div class="description">
                    Lorem Episum gray
                    spray master
                    livinu
                </div>
            </div>

            <div class="card">
                <h1>5</h1>
                <div class="description">
                    Lorem Episum gray
                    spray master
                    livinu
                </div>
            </div>
            
        </div>
    </div>
</template>

<script lang="ts">
export default {
    data () {
        return {

        }
    }
}
</script>

<style scoped>

.container {
    background: linear-gradient(261deg, #2a3b89 0%, #0e237e 48%, #2a3b89 100%);
    margin: 30px 0;
}

.dados {
    font-family: 'Poppins', sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 30px;
    display: flex;
}

.dados .card {
    width: 25%;
    height: 100px;
    margin: 0 30px;
    border-radius: 10px;
    display: flex;
    align-items: center;
    color: #fff;
    justify-content: center;
}

.dados .card h1 {
    padding: 15px;
    color: rgb(255, 226, 4);
}

.dados .card .description {
    font-size: 12px;
}
</style>