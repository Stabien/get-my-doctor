<script lang="ts">
	import { onMount } from 'svelte'
	import '../app.postcss'

	export const ssr = false

	const GOOGLE_MAPS_API = import.meta.env.VITE_GOOGLE_MAPS_API

	onMount(async () => (window.initMap = () => console.log('test')))
</script>

<svelte:head>
	<script
		defer
		async
		src="https://maps.googleapis.com/maps/api/js?key=${GOOGLE_MAPS_API}&callback=initmap"
	>
	</script>
</svelte:head>

<slot />
