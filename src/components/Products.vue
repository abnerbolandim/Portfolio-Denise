<template>
    <div id="app">
        <body>
            <section>
                <img src="../assets/wavesOpacity.svg" class="shape-divider" alt="">
                <div class="products-title">
                    <span >PRODUTOS</span>
                </div>
                <div class="row">
                    <div class="col-md-4 col-10">
                        <div class="card" style="">
                        <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">BOLO NO POTE</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-4 col-10">
                        <div class="card" style="">
                        <img src="../assets/SalgadosCard.jpg" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">SALGADINHOS</p>
                            </div>
                        </div>
                    </div> 
                </div>
                <div class="parallax-img"></div>
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
    /* padding: 25px; */
    background-color: #e8dddd;
}

body{
    font-family: Arial, sans-serif;
    box-sizing: unset;
}

.shape-divider{
    width: 100%;
}

.products-title{
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
    padding-bottom: 50px;
}

.card{
    border-style: none;
    margin: 20px;
    position: relative; 
    background-color: transparent;
}

.card-img-top {
    height: 500px; 
    object-fit: cover; 
    border-radius: 10px;
    transition: 0.5s;
}

.card-text {
    position: absolute;
    top: 50%; 
    left: 50%; 
    transform: translate(-50%, -50%); 
    color: black; 
    text-align: center;
    font-weight: 600;
    font-size: 17px;
    padding: 10px 20px; 
    background-color: rgba(255, 255, 255, 0.7);
    transition: 0.3s;
    width: 100%;
}

.card-text span{
    color: black;
    font-weight: 800;
}

.card:hover .card-text {
    color: white;
    background-color: #d8557b; 
}

@media (max-width: 768px) {
	.row {
        margin-right: calc(-7.5* var(--bs-gutter-x));
        margin-left: calc(-7.5* var(--bs-gutter-x));
	}
}

@media (max-width: 768px) {
	.row {
        margin-right: calc(-0.5* var(--bs-gutter-x));
        margin-left: calc(-0.5* var(--bs-gutter-x));
	}
}


.parallax-img {
    background-image: url("../assets/BoloShapeDivider01.jpg");

    min-height: 350px; 
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

</style>

