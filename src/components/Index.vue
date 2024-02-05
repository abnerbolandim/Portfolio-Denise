<template>
    <div id="app">
      <head>

        <link rel="icon" href="../assets/IconDenise.png">

      </head>
      <body>
        
        <header>
			<nav
				class="navbar navbar-expand-md navbar-light fixed-top navbar-transparent" 
				data-aos="fade-down"
				data-aos-offset="0"
				data-aos-duration="800"
			>
				<div class="container">
					<a href="index.html">
						<img class="ml-3 mt-1" src="images/Logo-Edson.svg" width="225" />
					</a>

					<button
						class="navbar-toggler mr-3"
						data-toggle="collapse"
						data-target="#nav-principal"
					>
						<i class="fas fa-bars text-white"></i>
					</button>

					<div class="ml-4 mt-2 navbar-collapse collapse" id="nav-principal">
						<ul class="navbar-nav ml-auto">
							<li class="nav-item">
								<a href="#portfolio h-100" class="nav-link">Home</a>
							</li>
							<li class="nav-item">
								<a href="#works" class="nav-link">Trabalhos</a>
							</li>
							<li class="nav-item">
								<a href="#about" class="nav-link">Sobre mim</a>
							</li>

							<li class="nav-item division"></li>

							<li class="nav-item">
								<a href="https://wa.me/5519989859294?text=Ol%C3%A1!%20Quero%20solicitar%20um%20or%C3%A7amento..." class="nav-link nav-contact"
									>Entre em contato agora
									<i class="ml-1 fa fa-whatsapp fa-1x"></i
								></a>
							</li>
						</ul>
					</div>
				</div>
			</nav>
		</header>

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
#portfolio {
	position: relative;
	height: 800px;
	margin-bottom: 20px;
}

.background-image {
	background-color: rgba(0, 0, 0, 0.5);
	height: 100vh;
	background-image: url("../assets/bolodepote.png");
	background-size: cover;
	background-position: center;

	margin-top: -50px;
}

.content {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	text-align: center;
	color: white;
}

.portfolio-title1 {
	font-size: 18px;
	margin-bottom: 15px;
	font-weight: 700;
	color: #f6f6f6;
	letter-spacing: -1px;
}

.portfolio-title2 {
	font-size: 39px;
	margin-bottom: 15px;
	font-weight: 700;
	color: #f6f6f6;
	letter-spacing: -0.5px;
}

.portfolio-title3 {
	font-size: 19px;
	margin-bottom: 10px;
	font-weight: lighter;
	color: #f6f6f6;
	letter-spacing: -0.3px;
}

</style>
