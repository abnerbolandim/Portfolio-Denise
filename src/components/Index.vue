<template>
    <div id="app">
      <head>



        <link rel="icon" href="../assets/IconDenise.png">

      </head>
      <body>
        
        <header>
			<nav
				class="navbar navbar-expand-md navbar-light fixed-top navbar-transparent" 
			
			>
				<div class="container">
					<a href="index.html">
						<img class="ml-3 mt-1" src="../assets/IconDenise.png" width="225" />
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

html,
body {
	overflow-x: hidden;
	scroll-behavior: smooth;
}

body {
	font-family: Arial, sans-serif;
	box-sizing: unset;
}


/* .navbar-collapse {
	display: none;
} */

.navbar-collapse.show {
	display: block;
}

nav.navbar-transparent {
	padding: 15px 0px;
	background: rgba(0, 0, 0, 0.6);
}

.navbar-light .navbar-nav .nav-link {
	color: white;
	transition: 0.3s;

}

.navbar-light .navbar-nav .nav-contact {
	color: #9feeaf;
}

.navbar-light .navbar-nav .nav-link:hover {
	color: #d3843d;
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
	background: white;
	margin: 12px 30px;
}

</style>
