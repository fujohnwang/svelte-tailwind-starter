<script>
	import SvelteLogo from 'virtual:icons/logos/svelte-icon';
	import AddressIcon from '~icons/ic/baseline-add-location-alt';  // import 'ic:baseline-add-location-alt' 

	let name = "svelte";

	let envSample = isProd;
	let host = mgtHost;
	let port = mgtPort;

	$:{
		console.log(`${host}:${port}`)
	}
</script>

<main>
	<div class="container mx-auto">

		<div class="flex py-24 justify-center">
			<div class="p-12 text-center max-w-2xl">
				<SvelteLogo/>
				<AddressIcon/>
				<h1 class="text-6xl font-bold">Hello {name}!</h1>
				<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p> 
			</div>
		</div>

	</div>
</main>

<style lang="postcss" global>
	@tailwind base;
	@tailwind components;
	@tailwind utilities;
</style>