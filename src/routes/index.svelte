
<style>
:root{
    background-color: #ecf5ff;
    font-size: 62.5%;
}

*{
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
    margin: 0;
    padding:0;
    color:#333;

}
h1,
h2,
h3,
h4  {
    margin-bottom: 1rem;

}
h1{
    font-size: 5.4rem;
    color:#56a5eb;
    margin-bottom: 5rem;
}

h1>span{
    font-size: 2.4rem;
    font-weight: 500;
}
h2{
    font-size: 4.2rem;
    margin-bottom: 4rem;
    font-weight: 700;
}
h3{
    font-size: 2.8rem;
    font-weight: 500;
}

/* herramientas*/

.container{
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 80 rem;
    margin:0 auto;
    padding:2rem;
}
.container>*{
    width: 100%;
}

.flex-column{
    display: flex;
    flex-direction: column;
}

.flex-center{
    justify-content: center;
    align-items: center;
}

.justify-center{
    justify-content: center;
}

.text-center{
    text-align: center;
}

.hidden{
    display: none;
}

/*botones*/

.btn{
    font-size: 1.8rem;
    padding: 1rem 0;
    width: 20rem;
    text-align: center;
    border: 0.1rem solid #56a5eb;
    margin-bottom: 1rem;
    text-decoration: none;
    color:#56a5eb;
    background-color: white;


}

.btn:hover{
    cursor:pointer;
    box-shadow: 0 0.4rem 0 rgba(86,185,235,0.5);
    transform: translateY(-0.1rem);
    transition: transform 150ms;
}

.btn [disabled]:hover{
    cursor:not-allowed;
    box-shadow: none;
    transform:none;
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
<div class="container">
  <div id="home" class="flex-center flex-column">
      <h1> Quick Quiz</h1>
     <a class="btn" href="game.svelte">Jugar</a>
     <a class="btn" href="highscores.svelte">High Scores</a>
  </div>
</div>





