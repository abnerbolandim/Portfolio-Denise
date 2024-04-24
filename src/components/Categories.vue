<template>
    <div id="app">
        <body>
            <section>
                <div class="categories-title">
                    <span >DESTAQUES</span>
                </div>
                <div class="row">
                    <div class="col-lg-4 col-10">
                        <div class="card" style="">
                        <img src="../assets/IconDeniseBlack.png" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">Sabor Morango - 2€</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-10">
                        <div class="card" style="">
                        <img src="../assets/IconDeniseBlack.png" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">Caixa c/ Salgadinhos - 3€</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-10">
                        <div class="card" style="">
                        <img src="../assets/IconDeniseBlack.png" class="card-img-top" alt="...">
                            <div class="card-body">
                                <p class="card-text">Sabor Paçoca - 2€</p>
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

.categories-title{
    text-align: center;
    color: #810947;
    font-size: 30px;
    font-weight: 600;
}

.card{
    border-style: none;
    margin: 20px;
}

.card img {
	max-width: 100%;
}

.card-text {
    text-align: center;
	font-size: 17px;
	margin-top: 15px;
	margin-left: 10px;
	margin-right: 10px;
}

</style>
