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

<section class="item-container">
	<header>
		<h3 class="subtitle">{name}</h3>
	</header>
	<Techonologies {techonologyNames} />
</section>
