<template>
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
                                <p class="card-text">sa,LFDSKNFHD</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-4 ">
                        <div class="card" style="">
                        <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">sa,LFDSKNFHD</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-4 ">
                        <div class="card" style="">
                        <img src="../assets/BoloCard01.jpg" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">sa,LFDSKNFHD</p>
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

@media (max-width: 750px) {
    .about-text {
        max-width: 90%;
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
}

.information01{
    padding-left: 60px;
}

.about-division {
    width: 2px;
    height: 200%; 
    background: #d8557b;
    margin: 0 12px;
    display: inline-block;
    vertical-align: middle; 
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



/* .row02{
    max-width: 1080px;
    margin: 0 auto;
    padding-bottom: 80px;
    display: flex;
	flex-wrap: wrap;

    margin-right: calc(0.5* var(--bs-gutter-x));
    margin-left: calc(0.5* var(--bs-gutter-x));
}

.caption-image{
    text-align: center;
}

.image-container {
    display: inline-block;
    position: relative;
    width: 300px;
    height: 200px;
    overflow: hidden;
    cursor: pointer;
}

@media (max-width: 991.5px) {
    .image-container {
        width: 500px;
        margin-right: calc(1* var(--bs-gutter-x));
        margin-left: calc(1* var(--bs-gutter-x));
    }
}

.image {
    width: 100%; 
    height: 100%; 
    z-index: 1;
    transition: all .5s;
}


.image img {
    width: 100%;
    height: auto;
}

.caption {
    width: 200px;
    height: auto;
    padding-top: 10px;
    padding-bottom: 10px;
    background: rgba(255, 255, 255, 0.8);
    z-index: 2;
    font-weight: 300;
    transition: all .5s;
}

.caption-01 {
    transform: translate(25%, 0%);
}

.image-container-01:hover .caption-01 {
    transform: translate(0%, -50%) translateY(-40%); 
    text-align: center;
}

.caption-02 {
        transform: translate(25%, 0%);
}

.image-container-01:hover .caption-02 {
     transform: translate(25%, -50%) translateY(-40%); 
     text-align: center;
}

.caption-03 {
    transform: translate(25%, 0%);
}

.image-container-01:hover .caption-03 {
     transform: translate(50%, -50%) translateY(-40%);
     text-align: center;
} */


</style>
