# How to create a button component using `Svelte` + `TailwindCSS`


## Step 1 - Create a new project using `SvelteKit`

    > npm init svelte@next WindyButton


## Step 2 - Add `TailwindCSS` using `svelte-add`

    > cd WindyButton
    > npx svelte-add@latest tailwindcss
    > npm install


## Step 3 - Create the component

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


## Step 4 - Use the component

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


## Step 5 - Witness the glory

![img](./res.png)

