<script>
	import { fly } from 'svelte/transition';
	import { SiGithub, SiPolygon } from '@icons-pack/svelte-simple-icons';
	import animax from '$lib/assets/animax-home.png';
	import rvgd from '$lib/assets/RVGD.png';
</script>

<div class="flex h-screen w-full flex-col items-center p-4">
	<div
		class="grid h-full w-full grid-flow-row-dense gap-4 lg:min-h-[500px] lg:max-w-[1250px] lg:grid-cols-4 lg:grid-rows-8"
	>
		<div
			in:fly={{ x: -50, duration: 300, delay: 600 }}
			out:fly={{ x: -50, duration: 300 }}
			class="bg-main flex items-center justify-center overflow-hidden rounded-3xl lg:col-span-2 lg:row-span-6"
		>
			<img src={animax} alt="animax | anime discovery web app" class="object-fit h-full w-full" />
		</div>
		<div
			in:fly={{ y: -50, duration: 300, delay: 600 }}
			out:fly={{ y: -50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl lg:col-span-2 lg:row-span-4"
		>
			<div class="relative h-full w-full p-4">
				<h1 class="mb-2 text-3xl font-semibold text-white">Animax</h1>
				<p class="text-white/75">
					Anime discovery web application. Uses the AniList API for data fetching. For this project,
					I set the limitation that I would not use any UI component libraries until completion of
					the first stage of development. Going forward I will incorporate Radix UI to enhance the
					UX and functionality of the project.
				</p>
				<div class="absolute bottom-0 flex justify-start gap-3 p-2">
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">TypeScript</p>
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">React</p>
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">Tailwindcss</p>
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">GraphQL</p>
				</div>
			</div>
		</div>
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl lg:col-span-1 lg:row-span-2"
		>
			<div class="text-white/75">
				<SiPolygon title="Link" size={60} />
			</div>
		</div>
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl lg:col-span-1 lg:row-span-2"
		>
			<div class="text-white/75">
				<SiGithub title="GitHub" size={60} />
			</div>
		</div>
	</div>

	<div
		class="grid h-full w-full grid-flow-row-dense gap-4 lg:min-h-[500px] lg:max-w-[1250px] lg:grid-cols-4 lg:grid-rows-8"
	>
		<div
			in:fly={{ x: -50, duration: 300, delay: 600 }}
			out:fly={{ x: -50, duration: 300 }}
			class="bg-main flex items-center justify-center overflow-hidden rounded-3xl lg:col-span-2 lg:row-span-6"
		>
			<img src={rvgd} alt="RVGD | videogame discovery web app" class="object-fit h-full w-full" />
		</div>
		<div
			in:fly={{ y: -50, duration: 300, delay: 600 }}
			out:fly={{ y: -50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl lg:col-span-2 lg:row-span-4"
		>
			<div class="relative h-full w-full p-4">
				<h1 class="mb-2 text-3xl font-semibold text-white">RVGD</h1>
				<p class="text-white/75">
					Videogame discovery web application. Uses the RAWG API for data fetching. Chakra UI
					component library is heavily used for designing the websites UI and functionality.
				</p>
				<div class="absolute bottom-0 flex justify-start gap-3 p-2">
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">TypeScript</p>
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">React</p>
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">Chakra UI</p>
					<p class="bg-highlight rounded-full px-2 py-1 text-sm text-white/75">REST API</p>
				</div>
			</div>
		</div>
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl lg:col-span-1 lg:row-span-2"
		>
			<div class="text-white/75">
				<SiPolygon title="Link" size={60} />
			</div>
		</div>
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl lg:col-span-1 lg:row-span-2"
		>
			<div class="text-white/75">
				<SiGithub title="GitHub" size={60} />
			</div>
		</div>
	</div>
</div>
