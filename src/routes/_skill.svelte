<script>
	export let name = 'Frontend Development';
	export let techonologyNames = [
		'React',
		'React Native',
		'Svelte',
		'Tailwind CSS',
		'Bootstrap',
		'Material Design'
	];
	import Techonologies from './_techonologies.svelte';
</script>

<section class="mb-4.5 break-inside-avoid">
	<header>
		<h3 class="text-lg font-semibold text-gray-700 leading-snugish">{name}</h3>
	</header>
	<Techonologies {techonologyNames} />
</section>
