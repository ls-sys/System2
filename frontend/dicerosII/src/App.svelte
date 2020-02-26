<script>
	export let name;
</script>

<main>

	<figure>
		<img src="diceros.jpg" alt="diceros">
		<figcaption>{name}</figcaption>
	</figure>
	
	<form action="https://diceros.ls-sys.com">
		<div>
			<span id="login">Inicio de Sesión</span>
		</div>
		<div>
			<label for="username">Nombre de Usuario</label>
			<input type="text" id="username" placeholder="Usuario">
		</div>
		
		<div>
			<label for="passphrase">Contraseña</label>
			<input type="password" id="passphrase" placeholder="Contraseña">
		</div>
		<div>
			<input type="submit" value="Iniciar Sesion">
		</div>
	</form>

</main>

<div class="cosmic1"></div>

<style>
	main {
		text-align: center;
		padding: 1rem;
		max-width: 600px;
		margin: 0 auto;
		font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}

	figure {
		margin-top: 1rem;
		margin-bottom: 2rem;
		width: auto;
		height: auto;
	}

	figure figcaption {
		color: #013467;
		text-transform: uppercase;
		font-size: 2.5em;
		font-weight: 100;
		margin-top: -1rem;
	}

	figure img {
		width: auto;
		height: 150px;
	}

	form {
		margin: auto;
		width: 350px;
		height: 250px;
		border: 1px solid black;
		padding: 30px 10px 45px 10px;
		border-radius: 8px;
		font-size: 14px;
		background-color: #f5faff;
	}

	form div {
		text-align: center;
		padding: 8px 4px;
	}

	form div:first-child{
		padding: 2px 4px 16px 4px;
		margin-top: 0;
	}

	form div span#login {
		font-family: inherit;
		font-weight: 400;
		font-size: 2em;
	}
	form div label {
		display: inline-block;
		text-align: left;
		font-size: 14px;
		color: #013467;
		width: 46%;
		display: none;
	}

	form div input:not([type='submit']) {
		display: block;
		border-top: 1px transparent;
		border-left: 1px transparent;
		border-right: 1px transparent;
		border-bottom: 1px solid #013467;
		margin: 0 auto;
		padding: 10px;
		outline: none;
		width: 60%;
		background-color: inherit;
	}

	form div input:not([type='submit'])::placeholder {
		color: #4188ce;
	}

	form div input[type='submit'] {
		padding: 10px 15px;
		margin-top: 20px;
		background-color: #b3d9ff;
		color: #013467;
		font-weight: 600;
		border: 0px solid transparent;
		cursor: pointer;
		outline: none;
	}

	.cosmic1 {
		width: 500px;
		z-index: -2;
		height: 800px;
		background-color: #4188ceb7;
		transform: rotate(78deg);
		position: absolute;
		top: 385px;
		left: 385px;
	}

	@media (min-width: 640px) {
		main {
			max-width: 100%;
		}
	}
</style>