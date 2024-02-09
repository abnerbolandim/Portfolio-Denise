<template>
    <div id="app">
      <head>
        <link rel="icon" href="../assets/IconDeniseBlack.png">
      </head>
      <body> 

		<div class="text-top-header">
			<a>FAÇA AGORA MESMO SEU <strong>PEDIDO ONLINE</strong></a>
		</div>

		<a href="index.html">
			<img class="denise-icon" src="../assets/IconDeniseBlack.png" width="225" />
		</a>

		<header class="d-flex">
			
			<nav class="navbar navbar-expand-md navbar-light navbar-transparent ">
				
				<div class="container justify-content-center">
					

					<div class="ml-md-auto navbar-collapse collapse" id="nav-principal">
						<ul class="navbar-nav">
							<li class="nav-item">
								<a href="index.html" class="nav-link">Home</a>
							</li>

							<li class="nav-item division"></li>

							<li class="nav-item dropdown">
								<a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
									Meus Trabalhos
								</a>
								<ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
									<li><a class="dropdown-item" href="#">Bolo no Pote</a></li>
									<li><a class="dropdown-item" href="#">Salgados</a></li>
								</ul>
							</li>

							<li class="nav-item division"></li>

							<li class="nav-item">
								<a href="#about" class="nav-link">Sobre mim</a>
							</li>

							<li class="nav-item division"></li>

							<li class="nav-item">
								<a href="https://wa.me/5519989859294?text=Ol%C3%A1!%20Quero%20solicitar%20um%20or%C3%A7amento..." class="nav-link nav-contact">Entre em contato agora <i class="ml-1 fa fa-whatsapp fa-1x"></i></a>
							</li>
						</ul>
					</div>
				</div>
			</nav>
		</header>


		<section>
			<div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
				<div class="carousel-indicators">
					<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
					<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
				</div>
				<div class="carousel-inner">
					<div class="carousel-item active">
						<img src="../assets/BoloCarousel.png" class="d-block w-100" alt="...">
					</div>
					<div class="carousel-item">
						<img src="../assets/SalgadosCarousel.png" class="d-block w-100" alt="...">
					</div>
				</div>
				<button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
					<span class="carousel-control-prev-icon" aria-hidden="true"></span>
					<span class="visually-hidden">Previous</span>
				</button>
				<button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
					<span class="carousel-control-next-icon" aria-hidden="true"></span>
					<span class="visually-hidden">Next</span>
				</button>
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
html,
body {
    overflow-x: hidden;
    scroll-behavior: smooth;
}

body {
	background-color: #fff0e8;
    font-family: Arial, sans-serif;
    box-sizing: unset;
}

.text-top-header {
	text-align: center;
	background-color: #810947;
	color: white;
	padding: 2px;
}

.denise-icon {
    display: block; 
    margin: 0 auto; 
    margin-bottom: 20px;
	margin-top: 20px;
}


.navbar {
    width: 100%;
	background-color: white;
}

.navbar-collapse {
    flex-grow: 0;
}

.navbar-collapse.show {
    display: block;
}

.navbar-light .navbar-nav .nav-link {
    font-size: large;
    color: rgb(59, 59, 59);
    transition: 0.3s;
}

.navbar-light .navbar-nav .nav-contact {
    color: #9feeaf;
}

.navbar-light .navbar-nav .nav-link:hover {
    color: #dd32ab;
    transform: scale(1.1);
}

.navbar-light .navbar-nav .nav-contact:hover {
    color: #1ad03f;
    transition: 0.3s;
    transform: scale(1.05);
}

.navbar-light .navbar-toggler {
    color: rgba(255, 255, 255, 0.5);
    border-color: rgba(255, 255, 255, 0.5);
}

.division {
    width: 1px;
    background: rgb(66, 66, 66);
    margin: 12px 12px;
}
</style>
