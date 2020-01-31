<script>
	export let name;
</script>

<main>

	<figure>
		<img src="#" alt="diceros">
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

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}

	figure {
		margin-top: 100px;
		margin-bottom: 40px;
	}

	figure figcaption {
		color: #013467;
		text-transform: uppercase;
		font-size: 3em;
		font-weight: 100;
	}

	form {
		margin: auto;
		width: 350px;
		height: 250px;
		border: 1px solid black;
		padding: 25px 15px;
		border-radius: 8px;
		font-size: 14px;
	}

	form div {
		text-align: center;
		padding: 5px 10px;
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
		margin: auto;
		padding: 10px;
		outline: none;
		width: 60%;
	}

	form div input:not([type='submit'])::placeholder {
		color: #4188ce;
	}

	form div input[type='submit'] {
		padding: 10px 15px;
		margin-top: 20px;
		background-color: #4188ce;
		color: #013467;
		font-weight: 600;
		border: 0px solid transparent;
		cursor: pointer;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>