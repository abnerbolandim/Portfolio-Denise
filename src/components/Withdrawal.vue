<template>
    <div id="app">
        <body>
            <section>
                <div class="card text-center">
                    <div class="card-body">
                        <h5 class="card-title">FAÇA SUA RETIRADA</h5>
                        <p class="card-text">Pedidos feitos até 12h podem ser retirados até 19h do mesmo dia.<br>
                                            Após este horário o prazo de retirar é até 1 dia útil até às 19h, após confirmação de pagamento.<br>
                                            Os pedidos com retirada agendada devem ser feitos com 1 dia de antecedência.</p>
                        <a href="#" class="btn" data-mdb-ripple-init>Contato</a>
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
    padding: 35px;
    background-color: #d8557b;
}

body{
    font-family: Arial, sans-serif;
    box-sizing: unset;
}

.card-body{
    background-color: #fbf2f2;
}

.card-title {
    letter-spacing: 0.5px;
    font-weight: bold;
    padding-top: 20px;
    font-size: 30px;
    color: #810947;
}

.card-text {
    letter-spacing: 0.7px;
    font-weight: 600;
    padding-top: 20px;
    font-size: 18px;
    color: #810947;
}


@media (max-width: 992px) {
    .card-title {
        font-size: 26px;
    }

    .card-text {
        font-size: 16px; 
    }
}


@media (max-width: 768px) {
    .card-title {
        font-size: 22px; 
    }

    .card-text {
        font-size: 14px; 
    }
}


@media (max-width: 576px) {
    .card-title {
        font-size: 20px; 
    }

    .card-text {
        font-size: 12px; 
    }
}

.btn {
    padding: 10px 20px 10px 20px;
    font-size: larger;
    color: white;
    background-color: #810947;
    shape-outside: none;
    transform: scale(1);
    transition: transform 0.3s ease; 
}

.btn:hover {
    color: rgb(222, 196, 229);
    background-color: #811a4f;
    shape-outside: none;
    transform: scale(1.1);
}
</style>
