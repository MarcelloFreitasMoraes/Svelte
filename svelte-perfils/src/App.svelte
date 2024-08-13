<script lang="ts">
	 let name: string = 'Marcelo';
	 let descricao: string = 'Esta é minha primeira aplicação com Svelte';
	 let src = 'https://img.freepik.com/fotos-gratis/close-up-de-um-gatinho-adoravel-no-sofa_23-2150782439.jpg'
	 let alt = 'Imagem de gato'
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>{descricao}</p>
	<img {src} {alt} height="300">
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>