<script lang="ts">
	import type { Opis } from './types';

	export let opis: Opis;
	const { name, image, description } = opis;
</script>

<div
	class="flex flex-col space-y-5 items-center font-black p-5 shadow-xl border-red-300 border-2 rounded-md bg-green-700 m-5 shadow-4xl"
>
	<h1 class="text-4xl">{name.toUpperCase()}</h1>
	<p class="text-sm">
		{description}
	</p>
	<img src={image} class="rounded-br-lg size-64" />
</div>
