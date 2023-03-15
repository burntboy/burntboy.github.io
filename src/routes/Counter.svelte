<script>
	let count = 0;
	let valueChanged = false;

	function handleClick() {
		count += 1;
		valueChanged = true;
	}
</script>

<div class="counter">
	<button on:click={handleClick}>
		Count is {count}
	</button>

	{#if valueChanged}
		<p>Value changed!</p>
	{/if}
</div>
