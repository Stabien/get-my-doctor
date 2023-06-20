<script lang="ts">
	import '../app.postcss'

	const GOOGLE_MAPS_API = import.meta.env.VITE_GOOGLE_MAPS_API

	console.log(GOOGLE_MAPS_API)

	window.initmap = () => console.log('test')
</script>

<svelte:head>
	<script
		defer
		async
		src="https://maps.googleapis.com/maps/api/js?key={GOOGLE_MAPS_API}&callback=initmap"
	>
	</script>
</svelte:head>

<slot />
