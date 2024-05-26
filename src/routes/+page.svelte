<script>
	const handleClick = () => {
		console.log('Boton click');
	};
</script>

<h1 class="text-2xl text-primary">Bienvenido a SvelteKit</h1>
<button on:click={handleClick} class="btn btn-primary mt-4">Boton</button>
<div class="form-control">
	<label class="label cursor-pointer">
		<span class="label-text">Remember me</span>
		<input type="checkbox" checked="checked" class="checkbox checkbox-primary" />
	</label>
</div>
<input type="radio" name="radio-2" class="radio radio-primary" checked />
<input type="radio" name="radio-2" class="radio radio-primary" />
