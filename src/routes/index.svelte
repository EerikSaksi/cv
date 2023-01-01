<script>
	import Experience from './_experience.svelte';
	import Project from './_project.svelte';
	import Skill from './_skill.svelte';
	import SectionContainer from './_section_container.svelte';
</script>

<main class="font-firago hyphens-manual">
	<!-- Page -->
	<div
		class="p-6 mx-auto page max-w-2xl print:max-w-a4 md:max-w-a4 md:h-letter xsm:p-8 sm:p-9 md:p-16 bg-white"
	>
		<header class="flex items-center mb-8 md:mb-11">
			<div
				class="initials-container mr-5 text-base leading-none text-white bg-gray-700 font-medium print:bg-black px-3"
				style="padding-bottom: 0.6875rem; padding-top: 0.6875rem; /*11px*/"
			>
				<div class="initial text-center" style="padding-bottom: 0.1875rem; /*3px*/">E</div>
				<div class="text-center initial">S</div>
			</div>
			<h1 class="text-2xl font-semibold text-gray-750 pb-px">Eerik Saksi</h1>
			<a href="https://eeriksak.si" class="group ml-4 text-gray-750">
				eeriksak.si
				<span class="link-arrow">↗</span>
			</a>
		</header>

		<!-- Column -->
		<div
			class="md:col-count-2 print:col-count-2 col-gap-md md:h-a4-col print:h-full  col-fill-auto"
		>
			<SectionContainer>
				<!-- To keep in the same column -->
				<div class="title-container">
					<h2 class="title">ABOUT ME</h2>

					<section class="item-container">
						<header>
							<h3 class="subtitle">Rust Developer</h3>
						</header>
						<p class="description">
							Passionate about WebAssembly and writing fast, safe and scalable servers/microservices
						</p>
					</section>
				</div>

				<section class="item-container">
					<header>
						<h3 class="subtitle">Fullstack Developer</h3>
					</header>
					<p class="description">
						Passionate about writing fast websites with minimal Javascript, cross platform mobile
						development, and automatic servers from databases
					</p>
				</section>
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
						'Worked on task automation',
						'Hosted meetings demonstrating automation task'
					]}
				/>
				<Experience
					company="Aalto University"
					timeRange="Aug 2022 – June 2023 | Software Developer"
					bulletPoints={[
						'Working on A+, an online learning platform for programming used by Aalto and other universities',
						'Working with Django, docker and Kubernetes',
						'Using pull requests to solve issues assigned at sprints'
					]}
				/>
			</SectionContainer>

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
					techonologyNames={[
						'Django',
						'Actix Web',
						'node.js',
						'TypeGraphQL/TypeORM',
						'Diesel',
						'MySQL',
						'Postgres',
						'SQLite',
						'MongoDB',
						'Neo4j'
					]}
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

			<SectionContainer>
				<!-- To keep in the same column -->
				<div class="title-container">
					<h2 class="title">CONTACT</h2>

					<section class="item-container">
						<ul class="list-inside pr-7">
							<li class="contact">saksi.eerik@gmail.com</li>
							<li class="contact">+358 40 669 1675</li>
							<li class="contact">
								<a href="https://www.linkedin.com/in/eerik-saksi-b58324193/" class="group">
									LinkedIn
									<span class="link-arrow">↗</span>
								</a>
							</li>
						</ul>
					</section>
				</div>
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
