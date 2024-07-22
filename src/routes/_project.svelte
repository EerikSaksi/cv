<script>
	import Techonologies from './_techonologies.svelte';
	export let name = 'Stat Buff';
	export let timeRange = 'Sep 2020 - May 2021';
	export let description =
		'Multiplayer iOS and Android fitness game. This app was designed to study the impacts of collaboration on exercise motivation. 30 users were surveyed and 10 interviewed.';
	export let href = 'https://github.com/EerikSaksi/stat_buff';
	export let techonologyNames = [
		'node.js',
		'Postgraphile',
		'Postgres',
		'React Native',
		'Typescript',
		'Apollo Client',
	];
</script>

<section class="item-container">
	<header>
		<h3 class="subtitle">
			<a {href} class="group">
				{name}
				<span class="link-arrow">↗</span>
			</a>

			<slot />
		</h3>
		<p class="time-range">{timeRange}</p>
	</header>
	<p class="description">
		{description}
	</p>
	<Techonologies {techonologyNames} />
</section>
