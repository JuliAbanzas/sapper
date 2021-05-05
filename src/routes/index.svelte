<script>

</script>
<style>
	h1, figure, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		font-family: monospace;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
		color:whitesmoke;
		
	}


	figure {
		margin: 0 0 1em 0;
	}

	img {
		border-radius: 50%;
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
		font-size: 170%;
		font-family:arial;
		font-weight: bold;
		color:azure;
		
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}

	.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
}
	.button {
  transition-duration: 0.4s;
}

.button:hover {
  background-color: #4CAF50; /* Green */
  color: white;
}
	
	</style>

<svelte:head>
	<title>La Caja Quiz App</title>
</svelte:head>

<h1>La Caja</h1>

<figure>
	<img alt='box' src='colorbox.jpg'>
	
</figure>
<button class="button button1">Iniciar Partida</button>
<button class="button button2">Registrarse</button>
<button class="button button3">Configuracion</button>
<button class="button button4">¿Cómo jugar?</button>




