<template>
    <div id="app">
        <body>
            <section>
                <div class="row">
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
                        <span class="information02">INGREDIENTE ÚNICO</span>
                        <span class="about-division"></span>
                        <span class="information03">CASEIRAMENTE ÚNICO</span>
                    </div>
                    
                </div>
                <div class="row">
                    <div class="caption-image col-md-4">
                        <div class="image-container image-container-01">
                            <div class="image image-01">
                                <img src="../assets/BoloCard01.jpg" />
                            </div>
                            <div class="caption caption-01">
                                TEST
                            </div>
                        </div>
                    </div>
                    <div class="caption-image col-md-4">
                        <div class="image-container image-container-01">
                            <div class="image image-01">
                                <img src="../assets/BoloCard01.jpg" />
                            </div>
                            <div class="caption caption-01">
                                TEST
                            </div>
                        </div>
                    </div>
                    <div class="caption-image col-md-4">
                        <div class="image-container image-container-01">
                            <div class="image image-01">
                                <img src="../assets/BoloCard01.jpg" />
                            </div>
                            <div class="caption caption-01">
                                TEST
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

.row{
    max-width: 1080px;
    margin: 0 auto;
    padding-bottom: 50px;
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

.caption-image{
    text-align: center;
}

.image-container {
  display: inline-block;
  position: relative;
  width: 300px;
  height: 200px;
  overflow: hidden;
  /* background: #fff; */
  cursor: pointer;
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
  transform: translateY(140px);
}

/* .image-container-01:hover .image-num2 {
  opacity: .8;
  transform: translateY(-50%) translateY(0px);
} */

.image-container-01:hover .caption-01 {
  transform: translateY(-37px);
  text-align: center;
}
</style>
