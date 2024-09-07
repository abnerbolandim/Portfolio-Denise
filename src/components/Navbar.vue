<template>
	<section id="navbar">
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
										<a href="index.html" class="nav-link">INÍCIO</a>
									</li>

									<li class="nav-item division"></li>

									<li class="nav-item dropdown">
										<a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
											PRODUTOS
										</a>
										<ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
											<li><a class="dropdown-item" href="#products">BOLO NO POTE</a></li>
											<li><a class="dropdown-item" href="#products">SALGADOS</a></li>
										</ul>
									</li>

									<li class="nav-item division"></li>


									<li class="nav-item">
										<a href="#about" class="nav-link">SOBRE</a>
									</li>


									<li class="nav-item division"></li>


									<li class="nav-item">
										<a href="#contact" class="nav-link">CONTATO</a>
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
								<img src="../assets/SalgadosCarousel.png" class="d-block w-100" alt="...">
							</div>
							<div class="carousel-item">
								<img src="../assets/BoloCarousel.png" class="d-block w-100" alt="...">
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
	</section>
</template>

<script>
export default {
  name: 'NavbarComponent',  
};
</script>

<style scoped>
html,
body {
    overflow-x: hidden;
    scroll-behavior: smooth;
}

body {
	background-color: #e8dddd;
    font-family: Arial, sans-serif;
    box-sizing: unset;
}

.text-top-header {
	text-align: center;
	background-color: #d8557b;
	color: white;
	padding: 2px;
}

.denise-icon {
    display: block; 
    margin: 0 auto; 
    padding: 10px;
}


.navbar {
    width: 100%;
	background-color: #d8557b;
}

.dropdown-item:hover{
	color: #ecb6dc;
}

.navbar-collapse {
    flex-grow: 0;
}

.navbar-collapse.show {
    display: block;
}

.navbar-light .navbar-nav .nav-link {
    font-size: large;
	font-weight: bold;
    color: white;
    transition: 0.2s;
}

.navbar-light .navbar-nav .nav-link:hover {
    color: #ecb6dc;
    transform: scale(1.1);
}

.navbar-light .navbar-toggler {
    color: rgba(255, 255, 255, 0.5);
    border-color: rgba(255, 255, 255, 0.5);
}

.division {
    width: 1px;
    background: white;
    margin: 12px 12px;
}


.carousel-inner img {
    width: 100%;
    height: auto; 
    object-fit: cover; 
}


@media (max-width: 768px) {
    .carousel-inner img {
        height: 300px; 
    }
}


@media (max-width: 576px) {
    .carousel-inner img {
        height: 200px; 
    }

    
    .carousel-indicators {
        bottom: -20px; 
    }

   
    .carousel-control-prev, .carousel-control-next {
        width: 30px; 
    }
}

</style>
