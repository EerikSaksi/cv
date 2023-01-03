<script>
	export let techonologyNames = [''];
</script>

<div class="my-3.2 last:pb-1.5">
	<ul class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6">
		{#each techonologyNames as techonologyName}
			<li
				class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 print:bg-white border-2 border-gray-300 rounded-md bg-gray-200"
			>
				{techonologyName}
			</li>
		{/each}
	</ul>
</div>
