# How to create a button component using `Svelte` + `Tailwind CSS`


## Step 1 - Create a new `SvelteKit` project with `Tailwind CSS` using `svelte-add`
    # Go through the interactive setup and choose Tailwind CSS
    > npm init @svelte-add/kit@latest
    # Or skip the process with this
    > npm init --yes @svelte-add/kit@latest WindyButton -- --with tailwindcss --demos false


## Step 2 - Create the component

    <!-- src/components/WindyButton.svelte -->
    
    <!-- Svelte event forwarding -->
    <button on:click >Click me!</button>
    <!-- Notice how you don't need to wrap the button in a div! -->
    
    <style>
      button {
        @apply bg-black text-white;
        @apply p-2 m-2;
        @apply font-bold;
        @apply border-2 rounded-md border-gray-200;
      }
    </style>


## Step 3 - Use the component

    <!-- src/routes/index.svelte -->
    
    <script>
    	import WindyButton from '../components/WindyButton.svelte';
    </script>
    
    <h1>Welcome to SvelteKit</h1>
    
    <WindyButton
    	on:click={() => {
    		console.log('WindyButton clicked!');
    	}}
    />


## Step 4 - Witness the glory

![img](./res.png)

