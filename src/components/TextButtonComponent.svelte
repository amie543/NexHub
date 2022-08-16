<script lang="ts">
	export let text : string= '';
	export let size : string = 'base';
	let style : string = "flex h-12 w-48 bg-indigo-900 justify-center items-center space-x-2 hover:shadow-lg hover:bg-indigo-800 rounded-md";
</script>

{#if size == 'base'}
	<div
		class={style}
	>
		<p class="text-white">{text}</p>
		<slot />
	</div>
{:else if size == 'sm'}
	<div
		class={style}
	>
		<p class="text-white">{text}</p>
		<slot />
	</div>
{/if}
