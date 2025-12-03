<script lang="ts">
    import type { PageProps } from '../counter/$types';

    let { data }: PageProps = $props();

    let count = $state(0)
</script>

<div class="border border-amber-500 rounded p-5 mx-auto my-auto w-1/2 xl:w-1/4 flex justify-between">
	<label for="counter" class="border-amber-500 bg-gray-950 border rounded w-1/2 flex justify-center items-center">{count}</label>
	<button
		class="bg-amber-500 text-gray-900 px-3 py-1 rounded-2xl font-bold"
		id="counter"
		onclick={() => {
			count++;
		}}>Count</button
	>
</div>
