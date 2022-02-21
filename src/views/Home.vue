<template>
	<main>

		<section id="home">
			<div data-aos="fade-up" data-aos-duration="1000">
				<h2>Bienvenidos a Krono Studios!</h2>
				<!--<p>Morbi semper rutrum augue, id consequat sapien porttitor et. Phasellus hendrerit mi sit amet lectus viverra lobortis.</p>-->
			</div>
			<a href="#about-us">Conoce más sobre nosotros <span>&darr;</span></a>
		</section>

		<section id="about-us">
			<img src="@/assets/about_us.jpg" alt="">
			<article data-aos="fade-left" data-aos-duration="750">
				<h2>Sobre nosotros</h2>
				<p>
					Kronos Studios es una empresa de creación de videojuegos que  busca innovar en la creación de videojuegos, lo mejor de todo es que su primer producto es un aplicativo móvil,  de esta forma buscamos estar más cerca de  nuestro público y acompañarlos en sus momentos de aburrimiento.
				</p>
				<p>
					Comenzamos la empresa con la idea de acompañar y brindar la mejor experiencia a los usuarios, cada proyecto se realiza pensando lo que quieren y desean los  clientes. Esta idea del nuevo videojuego nació después de la experiencia de los desarrolladores con otros juegos, es por ello que la empresa toma como prioridad las necesidades, deseos y demanda de los usuarios para los futuros proyectos.
				</p>
			</article>
		</section>

		<section id="our-team">
			<h2 data-aos="fade-right" data-aos-duration="750">Nuestro equipo</h2>
			<div class="team-cards">
				<div class="card" data-aos="fade-up" data-aos-duration="750">
					<img src="https://placekitten.com/250/350" alt="">
					<p class="name">Guillem Caballé Tomàs</p>
					<p>Founder | Fullstack dev</p>
					<p>Soy técnico superior en desarrollo de aplicaciones web y multiplataforma. Gamer desde pequeño.</p>
					<div class="socials">
						<a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
						<a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
					</div>
				</div>
				<div class="card" data-aos="fade-up" data-aos-duration="750" data-aos-delay="250">
					<img src="https://placekitten.com/250/350" alt="">
					<p class="name">Marc Fernández Parra</p>
					<p>Founder | Fullstack dev</p>
					<p>Soy desarrollador en Java con experiencia en android, y apasionado de los videojuegos.</p>
					<div class="socials">
						<a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
						<a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
					</div>
				</div>
				<div class="card" data-aos="fade-up" data-aos-duration="750" data-aos-delay="500">
					<img src="https://placekitten.com/250/350" alt="">
					<p class="name">Jimena Marin Ayoso</p>
					<p>Founder | Freelance en Innovación</p>
					<p>Soy estudiante en Ingenierìa y me considero buena en la planificación estratégica de las empresas.</p>
					<div class="socials">
						<a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
						<a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
					</div>
				</div>
				<div class="card" data-aos="fade-up" data-aos-duration="750" data-aos-delay="750">
					<img src="https://placekitten.com/250/350" alt="">
					<p class="name">Germán Pérez Bordera</p>
					<p>Founder | Fullstack dev</p>
					<p>Soy desarrollador web, siempre aprendiendo nuevas tecnologías y frameworks.</p>
					<div class="socials">
						<a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
						<a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
					</div>
				</div>
			</div>
		</section>

		<section id="our-project">
			<article data-aos="fade-right" data-aos-duration="750">
				<h2>Nuestro proyecto</h2>
				<p>
					El proyecto consiste en el desarrollo de un juego para dispositivos móviles con sistema
					android. El juego fusiona el género de cartas con un sistema de combate por turnos,
					dónde cada jugador creará su mazo y podrá personalizar su grupo de personajes. Cada
					carta representa una acción a ejecutar por uno de los personajes. Estos personajes
					disponen de unas estadísticas propias que afectan al efecto de la carta.
				</p>
				<p>
					El objetivo del juego será enfrentar el grupo del jugador con otro jugador o contra
					enemigos controlados por la máquina. Al cumplir este objetivo, el juego te recompensará
					con la moneda del juego que puedes gastar en comprar más cartas para mejorar tu
					mazo, y subir en la clasificación.
				</p>
			</article>
			<img src="@/assets/games.jpg" alt="">
		</section>

	</main>
</template>

<style scoped>
	main {
		display: flex;
		flex-direction: column;
	}
	section {
		min-height: 100vh;
		min-width: 100%;
	}
	h2 {
		font-size: 3rem;
		font-weight: 900;
		margin-bottom: 1rem;
	}
	#home {
		position: relative;
		background-color: whitesmoke;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	#home h2, #home p {
		text-align: center;
	}

	#home a {
		position: absolute;
		bottom: 2rem;
		left: 50%;
		transform: translateX(-50%);
		text-decoration: none;
	}

	#home a span {
		display: block;
		text-align: center;
		font-size: 3.5rem;
	}

	#about-us {
		position: relative;	
	}

	#about-us img {
		max-height: 600px;
		position: absolute;
		left: 50%;
		transform: translateX(-50%);
	}

	#about-us article {
		background-color: white;
		padding: 3rem;
		max-width: 400px;
		z-index: 5;
		position: absolute;
		right: 50px;
		top: 10rem;
	}
	
	article p {
		line-height: 1.5rem;
	}

	#our-team {
		padding-top: 7rem;
	}

	#our-team h2 {
		text-align: center;
	}

	#our-team .team-cards {
		display: flex;
		justify-content: center;
		flex-wrap: wrap;
		margin-top: 3rem;
		margin-bottom: 5rem;
	}

	#our-team .card {
		margin: 0 2rem;
		max-width: 290px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: start;
	}
	
	#our-team .card p {
		text-align: center;
		font-weight: 500;
		margin: .5rem 0;
	}

	#our-team .card p.name {
		margin-top: 1rem;
		font-weight: 900 !important;
	}
	
	#our-team .socials {
		margin-top: 1rem;
		display: flex;
		justify-content: center;
	}

	#our-team .socials a {
		margin: 0 1rem;
	}

	#our-project {
		position: relative;
	}

	#our-project article {
		background-color: white;
		padding: 3rem;
		max-width: 400px;
		z-index: 5;
		position: absolute;
		margin-left: 50px;
		margin-top: 10rem;
	}

	#our-project img {
		height: 450px;
		position: absolute;
		left: 50%;
		top: 50%;
		transform: translate(-50%, -50%);
		z-index: 1;
	}


</style>

<script>
	export default {
		name: 'Home',
		components: {
		}
	}
</script>