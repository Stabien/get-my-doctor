<script lang="ts">
	import { Input, Label } from 'flowbite-svelte'
	import type { InputType } from 'flowbite-svelte/dist/types'

	export let id: string
	export let type: InputType
	export let placeholder: string = ''
	export let label: string
</script>

<div>
	<Label for={id}>{label}</Label>
	<Input {type} {placeholder} />
</div>
