<script>
	import Techonologies from './_techonologies.svelte';

	export let name = 'Stat Buff';
	export let timeRange = 'Sep 2020 - May 2021';
	export let description =
		'Multiplayer iOS and Android fitness game. This app was designed to study the impacts of collaboration on exercise motivation. 30 users were surveyed and 10 interviewed.';
	export let href = 'https://github.com/EerikSaksi/stat_buff';
	export let techonologyNames = [
		'Postgraphile',
		'GraphQL',
		'Postgres',
		'React Native',
		'GraphQL Codegen',
		'Apollo Client',
		'React Native Paper',
		'React Navigation',
		'Typescript'
	];
</script>

<section class="mb-4.5 break-inside-avoid">
	<header>
		<h3 class="text-lg font-semibold text-gray-700 leading-snugish">
			<a {href} class="group">
				{name}
				<span
					class="inline-block text-gray-550 print:text-black font-normal group-hover:text-gray-700 transition duration-100 ease-in"
					>↗</span
				>
			</a>

			<slot />
		</h3>
		<p class="leading-normal text-md text-gray-650">{timeRange}</p>
	</header>
	<p class="mt-2.1 text-md text-gray-700 leading-normal">
		{description}
	</p>
	<Techonologies {techonologyNames} />
</section>
