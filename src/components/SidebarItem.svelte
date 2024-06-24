<script>
	import Icon from '@iconify/svelte'
	export let itemName
	export let itemIcon
	export let additionalData = ""
</script>

<div
	class="flex items-center justify-between cursor-pointer group gap-6 p-4 py-3 w-full rounded-full transition-all hover:bg-[var(--accent-color)]"
>
	<div
		class="flex items-center justify-center transition-all gap-4 group-hover:*:text-white"
	>
		<Icon
			class="text-2xl transition-all text-[var(--background-color)]"
			icon={itemIcon}
		/>
		<p class="text-xl transition-all text-[var(--background-color)] ">
			{itemName}
		</p>
	</div>
	{#if additionalData}
		<div class="bg-[var(--accent-color)] group-hover:bg-white group-hover:text-[var(--accent-color)] grid place-content-center rounded-full p-1 px-3 aspect-square text-white">{additionalData}</div>
	{:else}
		<Icon
			class="text-xl text-white "
			icon="octicon:chevron-right-12"
		/>
	{/if}
</div>
