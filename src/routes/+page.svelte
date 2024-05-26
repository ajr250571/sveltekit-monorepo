<script>
	let texto = '';
	const handleClick = () => {
		console.log('Boton click');
	};
</script>

<div class="flex flex-col w-96 justify-center">
	<h1 class="text-2xl text-primary">Bienvenido a SvelteKit</h1>
	<button on:click={handleClick} class="btn btn-primary mt-4">Boton</button>
	<div class="form-control">
		<label class="label cursor-pointer">
			<span class="label-text">Remember me</span>
			<input type="checkbox" checked="checked" class="checkbox checkbox-primary" />
		</label>
	</div>

	<input type="text" bind:value={texto} class="input input-primary" />
	<p>El texto tiene {texto.length} caracteres</p>
	{#if texto.length > 0}
		<button class="btn btn-secondary">Enviar Mensaje</button>
	{/if}
</div>
