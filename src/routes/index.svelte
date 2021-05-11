
<style>
	h1, figure {
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
  font-size: 20px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
  align-items: flex-start;
}
.button1 {
  background-color: white; 
  color: black; 
  border: 2px solid #4CAF50;
}

.button1:hover {
  background-color: #4CAF50;
  color: white;
}

.button2 {
  background-color: white; 
  color: black; 
  border: 2px solid #008CBA;
}

.button2:hover {
  background-color: #008CBA;
  color: white;
}

.button3 {
  background-color: white; 
  color: black; 
  border: 2px solid #f44336;
}

.button3:hover {
  background-color: #f44336;
  color: white;
}

.button4 {
  background-color: white;
  color: black;
  border: 2px solid #e7e7e7;
}

.button4:hover {background-color: #e7e7e7;}


	
	</style>

<svelte:head>
	<title>La Caja Quiz App</title>
</svelte:head>

  <h1>La Caja</h1>
  <script>
  import {currentUser} from './../stores/user.js'
  import Login from './../components/Login.svelte'
  </script>
  <h1>Great success {#if $currentUser}{$currentUser.displayName}{/if}! </h1>
  <Login />
<figure>
	<img alt='box' src='blackbox.jpg'>
	
</figure>
<div>
  <button class="button button1">Iniciar Partida</button>
<button class="button button2">Registrarse</button>
<button class="button button3">Configuracion</button>
<button class="button button4">¿Cómo jugar?</button>
</div>





