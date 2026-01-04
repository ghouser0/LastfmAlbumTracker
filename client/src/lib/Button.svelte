<script>
	export let type = 'primary';
	export let flat = false;
</script>


<button class={type} class:flat={flat}>
	<slot></slot>
</button>


<style>
	button {
		border: 0;
		cursor: pointer;
		border-radius: 6px;
		padding: 8px 12px;
		font-weight: bold;
		box-shadow: 1px 2px 3px rgba(25, 25, 25, .2);
	}

	.primary {
		background: rgba(134, 68, 73, 1);
		color: white;
	}

	.secondary {
		background: rgba(167, 191, 205, 1);
		color: black;
	}

	.flat {
		box-shadow: none;
	}
</style>
