<script>
	export let company = 'UROS';
	export let timeRange = 'Jun 2019 – Aug 2019 | Software Engineer Intern';
	export let bulletPoints = [
		'Reverse engineered existing homogenous codebase into one Python solution',
		'Maintained backwards compatibility with existing customer data'
	];
</script>

<section class="item-container">
	<header>
		<h3 class="subtitle">{company}</h3>
		<p class="time-range">
			{timeRange}
		</p>
	</header>
	<ul class="">
		{#each bulletPoints as bulletPoint}
			<li class="description">
				<span class="absolute -ml-3 sm:-ml-3.2 select-none transform -translate-y-px">›</span>
                {bulletPoint}
			</li>
		{/each}
	</ul>
</section>
