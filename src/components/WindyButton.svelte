<script>
	export let buttonText = 'Click me!';
	// Passing in props
</script>

<!-- Svelte event forwarding -->
<button on:click>
	{buttonText}
</button>

<!-- Notice how you don't need to wrap the button in a div! -->
<style>
	button {
		@apply bg-black text-white;
		@apply p-2 m-2;
		@apply font-bold;
		@apply border-2 rounded-md border-gray-200;
	}
</style>
