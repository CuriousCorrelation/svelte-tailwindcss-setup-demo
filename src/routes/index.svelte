<script>
	import WindyButton from '../components/WindyButton.svelte';
</script>

<WindyButton
	on:click={() => {
		console.log('WindyButton clicked!');
	}}
/>

<WindyButton
	buttonText={'No, click me!'}
	on:click={() => {
		console.log('Other WindyButton clicked!');
	}}
/>
