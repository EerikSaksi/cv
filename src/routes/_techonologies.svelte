<script>
	export let techonologyNames = [''];
</script>

<div class="my-3.2 last:pb-1.5">
	<ul class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6">
		{#each techonologyNames as techonologyName}
			<li
				class="px-2.5 mr-1.6 mb-1.6  print:bg-white print:border-inset  subtitle-overrides rounded-full border-overrides "
			>
				{techonologyName}
			</li>
		{/each}
	</ul>
</div>
