<template>
    <div id="app">
        <body>
            <section>
                <div class="categories-title">
                    <span >DESTAQUES</span>
                </div>
                <div class="row">
                    <div class="col-10 mx-auto">
                        <div id="carouselExampleControls" class="carousel slide d-md-none" data-bs-ride="carousel">
                        <div class="carousel-inner">
                            <div class="carousel-item active">
                            <div class="card">
                                <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                <p class="card-text">Sabor Morango<br><span>€ 2.00</span></p>
                                </div>
                            </div>
                            </div>
                            <div class="carousel-item">
                            <div class="card">
                                <img src="../assets/SalgadosCard.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                <p class="card-text">Caixa c/ Salgadinhos<br><span>€ 3.00</span></p>
                                </div>
                            </div>
                            </div>
                            <div class="carousel-item">
                            <div class="card">
                                <img src="../assets/BoloCard02.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                <p class="card-text">Sabor Paçoca<br><span>€ 2.00</span></p>
                                </div>
                            </div>
                            </div>
                        </div>
                        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Anterior</span>
                        </button>
                        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Próximo</span>
                        </button>
                        </div>
                    </div>
                    <div class="col-md-4 d-md-block d-none">
                        <div class="card">
                        <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="card-text">Sabor Morango<br><span>€ 2.00</span></p>
                        </div>
                        </div>
                    </div>
                    <div class="col-md-4 d-md-block d-none">
                        <div class="card">
                        <img src="../assets/SalgadosCard.jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="card-text">Caixa c/ Salgadinhos<br><span>€ 3.00</span></p>
                        </div>
                        </div>
                    </div>
                    <div class="col-md-4 d-md-block d-none">
                        <div class="card">
                        <img src="../assets/BoloCard02.jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="card-text">Sabor Paçoca<br><span>€ 2.00</span></p>
                        </div>
                        </div>
                    </div>
                </div>
            </section>
        </body>
    </div>
</template>

<script>
export default {
  name: 'App',
  props: {
  }
}
</script>

<style scoped>
#app{
    font-family: Arial, sans-serif;
    justify-content: center;
    padding: 25px;
    background-color: white;
}

body{
    font-family: Arial, sans-serif;
    box-sizing: unset;
}

.categories-title{
    letter-spacing: 0.5px;
    text-align: center;
    color: #810947;
    font-size: 30px;
    font-weight: 600;
    padding-top: 40px;
    padding-bottom: 15px;
}

.row {
    justify-content: center;
}

.card{
    border-style: none;
    margin: 20px;
}

.card-img-top {
    height: 300px; 
    object-fit: cover; 
    border-radius: 30px;
    transition: 0.5s;
}

.card-img-top:hover {
    transform: scale(1.05);
}

.card-text {
    color: #810947;
    text-align: center;
    font-weight: 600;
	font-size: 17px;
	margin-top: 5px;
	margin-left: 10px;
	margin-right: 10px;
    transition: 0.5s;
}

.card-text span{
    color: black;
    font-weight: 800;
}

@media (min-width: 992px) {
	.row {
        margin-right: calc(2.5* var(--bs-gutter-x));
        margin-left: calc(2.5* var(--bs-gutter-x));
	}
}
</style>
