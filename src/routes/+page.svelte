<script lang="ts">
	import InputAddress from '../components/InputAddress.svelte'
	import InputSpecialization from '../components/InputSpecialization.svelte'
</script>

<main class="flex justify-center">
	<div class="search-input flex flex-row justify-center mt-10 w-1/2">
		<div class="w-full mr-2">
			<InputAddress />
		</div>
		<div class="w-full ml-2">
			<InputSpecialization />
		</div>
	</div>
</main>
