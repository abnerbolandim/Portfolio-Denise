<template>
    <section id="about">
        <div id="app">
            <body>
                <section>
                    <div class="row row01">
                        <div class="about-title">
                            <span >SOBRE MIM</span>
                        </div>

                        <div class="about-text01">
                            <span >A DENISE Bolos & Salgados nasceu com produtos para você 
                                experimentar e apreciar o 
                                melhor da caseira confeitaria brasileira.</span>
                        </div>
                        <div class="about-text02"><span>Além do mais nossas bases, recheios, coberturas e 
                                salgadinhos são feitas artesanalmente para que você possa 
                                desfrutar do melhor!</span></div>

                        <div class="about-information">
                            <span class="information01">SABOR ÚNICO</span>
                            <span class="about-division"></span>
                            <span class="information02">CASEIRAMENTE ÚNICO</span>
                            <span class="about-division"></span>
                            <span class="information03">INGREDIENTE ÚNICO</span>
                        </div>
                        
                    </div>
                    <div class="row">
                        <div class="col-md-4 ">
                            <div class="card" style="">
                            <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                    <p class="card-text text01">ESPECIALMENTE</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 ">
                            <div class="card" style="">
                            <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                    <p class="card-text text02">PENSADO</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 ">
                            <div class="card" style="">
                            <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                    <p class="card-text text03">EM VOCÊ!</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="parallax-img"></div>
                </section>
            </body>
        </div>
    </section>
</template>

<script>
export default {
  name: 'AboutComponent',
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

.row01{
    max-width: 1080px;
    margin: 0 auto;
    padding-bottom: 80px;
}

.shape-divider{
    width: 100%;
}

.about-title{
    letter-spacing: 0.5px;
    text-align: center;
    color: #810947;
    font-size: 30px;
    font-weight: 600;
    padding-top: 70px;
    padding-bottom: 15px;
}

.about-text01{
    margin: 0 auto; 
    max-width: 70%;
    text-align: center;
    color: black;
    font-size: 17px;
    font-weight: 600;
    padding-top: 18px;
    padding-bottom: 15px;
}

.about-text02{
    margin: 0 auto; 
    max-width: 70%;
    text-align: center;
    color: black;
    font-size: 17px;
    font-weight: 600;
    padding-bottom: 15px;
}

@media (max-width: 700px) {
    .about-text01 {
        max-width: 95%;
    }
    .about-text02 {
        max-width: 95%;
    }
}


.about-information {
    padding-top: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #d8557b;
    font-size: 17px;
    font-weight: 600;
    flex-wrap: wrap; 
}

.about-information span {
    margin: 7px;
    padding: 7px 1px; 
}

.about-division {
    width: 2px;
    height: 100%; 
    background: #d8557b;
    display: inline-block;
    vertical-align: middle;
}

.information01, .information02, .information03 {
    padding-left: 0;
}

@media (max-width: 700px) {
    .about-information {
        flex-direction: column; 
    }

    .about-division {
        width: 70%; 
        height: 2px; 
        margin: 12px 0; 
    }

    .about-information span {
        padding: 1px 10px; 
    }
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
    top: 100%; 
    left: 50%; 
    transform: translate(-50%, -50%); 
    color: black; 
    text-align: center;
    font-weight: 600;
    font-size: 17px;
    padding: 10px 20px; 
    /* background-color: rgba(255, 255, 255, 0.7); */
    border-radius: 12px;
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
    letter-spacing: 1.3px; 
}

.card:hover .text01{
    left: 0%;
    position: absolute;
    top: 80%;
    color: rgb(255, 255, 255);
    background-color: #d8557b;
    letter-spacing: 1.3px;
    transform: rotate(0deg);
}

.card:hover .text02{
    left: 0%;
    position: absolute;
    top: 70%;
    color: rgb(255, 255, 255);
    background-color: #d8557b;
    letter-spacing: 1.5px;
    transform: rotate(0deg);
}

.card:hover .text03{
    left: 0%;
    position: absolute;
    top: 80%;
    color: rgb(255, 255, 255);
    background-color: #d8557b;
    letter-spacing: 1.3px;
    transform: rotate(0deg);
}

@media (max-width: 800px) {
	.row {
        margin-right: calc(-7.5* var(--bs-gutter-x));
        margin-left: calc(-7.5* var(--bs-gutter-x));
	}
}

@media (max-width: 800px) {
	.row {
        margin-right: calc(-0.5* var(--bs-gutter-x));
        margin-left: calc(-0.5* var(--bs-gutter-x));
	}
}

.parallax-img {
    margin-top: 50px;
    background-image: url("../assets/BoloShapeDivider02.jpg");

    min-height: 350px; 
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

</style>
