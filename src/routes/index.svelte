<script>
	import Experience from './_experience.svelte';
	import Project from './_project.svelte';
	import Skill from './_skill.svelte';
</script>

<main class="font-firago hyphens-manual">
	<!-- Page -->
	<div
		class="p-6 mx-auto page max-w-2xl print:max-w-a4 md:max-w-a4 md:h-letter xsm:p-8 sm:p-9 md:p-16 bg-white"
	>
		<!-- Name -->
		<header class="flex items-center mb-8 md:mb-11">
			<div
				class="initials-container mr-5 text-base leading-none text-white bg-gray-700 font-medium print:bg-black px-3"
				style="padding-bottom: 0.6875rem; padding-top: 0.6875rem; /*11px*/"
			>
				<div class="initial text-center" style="padding-bottom: 0.1875rem; /*3px*/">E</div>
				<div class="text-center initial">S</div>
			</div>
			<h1 class="text-2xl font-semibold text-gray-750 pb-px">Eerik Saksi</h1>
		</header>
		<!-- end Name -->

		<!-- Column -->
		<div
			class="md:col-count-2 print:col-count-2 col-gap-md md:h-a4-col print:h-a4-col col-fill-auto"
		>
			<section class="mt-8 first:mt-0">
				<!-- To keep in the same column -->
				<div class="break-inside-avoid">
					<h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal">
						ABOUT ME
					</h2>

					<section class="mb-4.5 break-inside-avoid">
						<header>
							<h3 class="text-lg font-semibold text-gray-700 leading-snugish">Rust Developer</h3>
						</header>
						<p class="mt-2.1 text-md text-gray-700 leading-normal">
							Passionate about WebAssembly and writing fast, safe and scalable servers/microservices
						</p>
					</section>
				</div>

				<section class="mb-4.5 break-inside-avoid">
					<header>
						<h3 class="text-lg font-semibold text-gray-700 leading-snugish">Fullstack Developer</h3>
					</header>
					<p class="mt-2.1 text-md text-gray-700 leading-normal">
						Passionate about writing fast websites with minimal javascript, cross platform mobile
						development, and automatic servers from databases
					</p>
				</section>
			</section>

			<section class="mt-8 first:mt-0">
				<!-- To keep in the same column -->
				<div class="break-inside-avoid">
					<h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal">
						EXPERIENCE
					</h2>
					<Experience />
				</div>

				<Experience
					company="Barclays UK"
					timeRange="Jun 2021 – Aug 2021 | Technology Developer Intern"
					bulletPoints={['Worked in techonology resillience and incident management']}
				/>
			</section>

			<section class="mt-8 first:mt-0">
				<!-- To keep in the same column -->
				<div class="break-inside-avoid">
					<h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal">
						EDUCATION
					</h2>

					<section class="mb-4.5 break-inside-avoid">
						<header>
							<h3 class="text-lg font-semibold text-gray-700 leading-snugish">
								University of Glasgow
							</h3>
							<p class="leading-normal text-md text-gray-650">
								2018 – 2022 | Master's Degree in Computing
							</p>
						</header>
					</section>
				</div>
			</section>

			<section class="mt-8 first:mt-0">
				<!-- To keep in the same column -->
				<div class="break-inside-avoid">
					<h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal">
						PROJECTS
					</h2>
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
			</section>
			<Project
				name="Postgrustql"
				timeRange="Sep 2021 - May 2022"
				description="Postgrustql transforms a Postgres database into a GraphQL server accepting read and writes automatically. This project was designed to compete with existing projects such as Postgraphile and Hasura."
				techonologyNames={['Rust', 'Actix Web', 'GraphQL', 'Postgres']}
			/>

			<section class="mt-8 first:mt-0">
				<!-- To keep in the same column -->
				<div class="break-inside-avoid">
					<h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal">
						SKILLS
					</h2>
				</div>
				<Skill />

				<Skill
					name="Backend Development"
					techonologyNames={[
						'Django',
						'Actix Web',
						'node.js',
						'MySQL',
						'Postgres',
						'TypeGraphQL/Typeorm'
					]}
				/>

				<Skill
					name="Data Science"
					techonologyNames={['Pandas', 'scikit-learn', 'SQLAlchemy', 'Spotlight', 'Matplotlib']}
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
			</section>

			<section class="mt-8 first:mt-0">
				<!-- To keep in the same column -->
				<div class="break-inside-avoid">
					<h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-550 print:font-normal">
						CONTACT
					</h2>

					<section class="mb-4.5 break-inside-avoid">
						<ul class="list-inside pr-7">
							<li class="mt-1.5 leading-normal text-gray-700 text-md">
								<a href="//webpraktikos.com" class="group">
									webpraktikos.com
									<span
										class="inline-block text-gray-550 print:text-black font-normal group-hover:text-gray-700 transition duration-100 ease-in"
										>↗</span
									>
								</a>
							</li>
							<li class="mt-1.5 leading-normal text-gray-700 text-md">
								<a href="//twitter.com/webpraktikos" class="group">
									twitter.com/webpraktikos
									<span
										class="inline-block text-gray-550 print:text-black font-normal group-hover:text-gray-700 transition duration-100 ease-in"
										>↗</span
									>
								</a>
							</li>
							<li class="mt-1.5 leading-normal text-gray-700 text-md">1020 Wien, Austria</li>
							<li class="mt-1.5 leading-normal text-gray-700 text-md">hi@webpraktikos.com</li>
							<li class="mt-1.5 leading-normal text-gray-700 text-md">(+43) 0699 77 33 77 55</li>
						</ul>
					</section>
				</div>
			</section>
		</div>
		<!-- end Column -->
	</div>
	<!-- end Page -->
</main>
