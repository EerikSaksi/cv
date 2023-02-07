<script>
	import Experience from './_experience.svelte';
	import Project from './_project.svelte';
	import Skill from './_skill.svelte';
	import SectionContainer from './_section_container.svelte';
</script>

<svelte:head>
	<link
		rel="stylesheet"
		href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/default.min.css"
	/>
	<script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js">
	</script>
</svelte:head>

<main class="font-firago hyphens-manual">
	<!-- Page -->
	<div
		class="p-6 mx-auto page max-w-2xl print:max-w-a4 md:max-w-a4 md:h-letter xsm:p-8 sm:p-9 md:p-16 bg-white"
	>
		<header class="flex items-center mb-1">
			<h1 class="text-2xl font-semibold text-gray-750 pb-px mr-3">EERIK SAKSI</h1>
			<code
				class="language-bash s-Uap-jPRb-uiE hljs bg-white border-2 border-2 border-gray-300 rounded-md text-gray-750"
				><span class="hljs-built_in ">echo</span> <span class="hljs-variable">$FIRST_NAME</span> | sed
				s/E/EE</code
			>
		</header>
		<header class="flex items-center mb-4 md:mb-8">
			<div class="border-b-4 border-gray-300 border-dotted">
				<a href="https://eeriksak.si" class="group text-gray-750">
					eeriksak.si
					<span class="link-arrow">↗</span>
				</a>
				<a href="mailto:saksi.eerik@gmail.com" class="group ml-4 text-gray-750">
					saksi.eerik@gmail.com
					<span class="link-arrow">↗</span>
				</a>
				<a href="tel:44 7519 698 702" class="group ml-4 text-gray-750">
					+44 7519 698 702
					<span class="link-arrow">↗</span>
				</a>
				<a
					href="https://www.linkedin.com/in/eerik-saksi-b58324193/"
					class="group ml-4 text-gray-750"
				>
					LinkedIn
					<span class="link-arrow">↗</span>
				</a>
				<a
					href="https://github.com/EerikSaksi"
					class="group ml-4 text-gray-750"
				>
					GitHub
					<span class="link-arrow">↗</span>
				</a>
			</div>
		</header>

		<!-- Column -->
		<div
			class="md:col-count-2 print:col-count-2 col-gap-md md:h-a4-col print:h-full  col-fill-auto"
		>
			<SectionContainer>
				<!-- To keep in the same column -->
				<div class="title-container">
					<h2 class="title">EDUCATION</h2>
				</div>

				<Experience
					company="University of Glasgow"
					timeRange="2018 – 2022 | Master's Degree in Computing"
					bulletPoints={['First Class Honours with 2nd Year Entry']}
				/>
			</SectionContainer>
			<SectionContainer>
				<!-- To keep in the same column -->
				<div class="title-container">
					<h2 class="title">EXPERIENCE</h2>
					<Experience />
				</div>

				<Experience
					company="Barclays UK"
					timeRange="Jun 2021 – Aug 2021 | Technology Developer Intern"
					bulletPoints={[
						'Worked in technology resillience and incident management',
						'Automated sending emails by formatting Oracle Database data into HTML'
					]}
				/>
				<Experience
					company="Aalto University"
					timeRange="Aug 2022 – June 2023 | Software Developer"
					bulletPoints={[
						'Working on A+, an online learning platform for programming used by Aalto and other universities',
						'Django, Docker, Kubernetes',
						'Agile Development with sprints, pull requests, and code review'
					]}
				/>
			</SectionContainer>

			<SectionContainer>
				<!-- To keep in the same column -->
				<div class="title-container">
					<h2 class="title">PROJECTS</h2>
					<Project>
						<div class="flex my-1">
							<a href="https://play.google.com/store/apps/details?id=com.statbuff">
								<img
									class="h-6 mr-2"
									src="https://www.freepnglogos.com/uploads/google-play-png-logo/google-play-logo-google-play-game-google-play-store-app-00.jpg"
									alt=""
								/>
							</a>

							<a
								href="https://web.archive.org/web/20210831133805/https://apps.apple.com/iq/app/stat-buff/id1551529468"
							>
								<img
									class="h-6"
									src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Apple_Store_logo.svg/1024px-Apple_Store_logo.svg.png"
									alt=""
								/>
							</a>
						</div>
					</Project>
				</div>
			</SectionContainer>
			<Project
				name="Poggers"
				timeRange="Sep 2021 - May 2022"
				description="Poggers automatically generates GraphQL middleware for a Postgres database. Designed with performance and scalability in mind, it outperforms Hasura and Postgraphile."
				techonologyNames={[
					'Rust',
					'Actix Web',
					'GraphQL',
					'Postgres',
					'Tokio',
					'async-graphql',
					'petgraph',
					'serde',
					'Docker'
				]}
				href="https://github.com/EerikSaksi/poggers"
			/>

			<SectionContainer>
				<!-- To keep in the same column -->
				<div class="title-container">
					<h2 class="title">SKILLS</h2>
				</div>
				<Skill />

				<Skill
					name="Backend Development"
					techonologyNames={['Django', 'Actix Web', 'node.js', 'TypeGraphQL/TypeORM', 'Diesel']}
				/>
				<Skill
					name="Databases"
					techonologyNames={['MySQL', 'Postgres', 'SQLite', 'MongoDB', 'Neo4j', 'Dgraph', 'IndraDB']}
				/>

				<Skill
					name="Data Science"
					techonologyNames={[
						'Pandas',
						'scikit-learn',
						'SQLAlchemy',
						'Spotlight',
						'Matplotlib',
						'Tesseract'
					]}
				/>
				<Skill
					name="Cloud"
					techonologyNames={['Heroku', 'Apex', 'AWS RDS', 'Firebase Authentication', 'Vercel']}
				/>
				<Skill
					name="Other"
					techonologyNames={[
						'Haskell',
						'Java',
						'C/C++',
						'Python',
						'Linux/Bash',
						'AMD64 Assembly',
						'User Centered Design',
						'Test Driven Development',
						'Scrum'
					]}
				/>
			</SectionContainer>
		</div>
		<!-- end Column -->
	</div>
	<!-- end Page -->
</main>

<style lang="postcss" global>
	.title {
		@apply mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal;
	}
	.contact {
		@apply mt-1.5 leading-normal text-gray-700 text-md;
	}
	.subtitle {
		@apply text-lg font-semibold text-gray-700 leading-snugish;
	}
	.link-arrow {
		@apply inline-block text-gray-550 print:text-black font-normal group-hover:text-gray-700 transition duration-100 ease-in;
	}
	.description {
		@apply mt-2.1 text-md text-gray-700 leading-normal;
	}
	.time-range {
		@apply leading-normal text-md text-gray-650;
	}
	.title-container {
		@apply break-inside-avoid;
	}
	.item-container {
		@apply mb-4.5 break-inside-avoid;
	}
</style>
