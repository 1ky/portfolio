<script>
	import { fly, fade } from 'svelte/transition';
	import {
		SiArchlinux,
		SiCss3,
		SiGit,
		SiGithub,
		SiGraphql,
		SiHtml5,
		SiJavascript,
		SiMongodb,
		SiMysql,
		SiPython,
		SiReact,
		SiSvelte,
		SiTailwindcss,
		SiTypescript
	} from '@icons-pack/svelte-simple-icons';
	import shibuya from '$lib/assets/shibuya-crossing.jpg';
	import me from '$lib/assets/myself.jpg';
</script>

<div class="mb-10 flex h-screen w-full items-center justify-center p-4">
	<div
		class="grid h-full w-full grid-flow-row-dense grid-cols-1 gap-4 lg:max-w-[1250px] lg:grid-cols-10 lg:grid-rows-4"
	>
		<!-- Github grid -->
		<div
			in:fly={{ x: -50, duration: 300, delay: 600 }}
			out:fly={{ x: -50, duration: 300 }}
			class="lg:row-span- bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-2"
		>
			<div class="flex flex-col items-center justify-center gap-2 hover:text-white">
				<a href="https://github.com/1ky/">
					<SiGithub title="GitHub" size={60} />
				</a>
				<div class="flex flex-col items-center justify-center">
					<h2 class="text-sm text-white/50">github.com/1ky</h2>
				</div>
			</div>
		</div>

		<!-- Developer grid -->
		<div
			in:fly={{ x: -50, duration: 300, delay: 600 }}
			out:fly={{ x: -50, duration: 300 }}
			class="flex items-center justify-center rounded-3xl bg-amber-300/50 text-white/75 lg:col-span-4 lg:row-span-1"
		>
			<h2 class="p-4 text-3xl font-semibold text-white">Frontend/Full Stack Developer</h2>
		</div>

		<!-- Decorative image 1 -->
		<div
			in:fly={{ y: -50, duration: 300, delay: 600 }}
			out:fly={{ y: -50, duration: 300 }}
			class="bg-main hidden items-center justify-center overflow-hidden rounded-3xl text-white/75 lg:col-span-2 lg:row-span-2 lg:flex"
		>
			<img src={me} alt="Kyle Shepherd" class="h-full w-full object-cover" />
		</div>

		<!-- Specialties grid -->
		<div
			in:fly={{ y: -50, duration: 300, delay: 600 }}
			out:fly={{ y: -50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-2 lg:row-span-2"
		>
			<div class="flex flex-col items-center justify-center">
				<h2 class="p-4 text-3xl font-semibold text-white">Technologies</h2>
				<div class="flex flex-wrap gap-3 p-8 *:cursor-pointer *:text-white/50 *:hover:text-white">
					<SiHtml5 title="HTML" />
					<SiCss3 title="CSS" />
					<SiJavascript title="JavaScript" />
					<SiTypescript title="TypeScript" />
					<SiPython title="Python" />
					<SiReact title="React" />
					<SiSvelte title="Svelte" />
					<SiTailwindcss title="Tailwindcss" />
					<SiGit title="Git" />
					<SiArchlinux title="Arch Linux" />
					<SiMysql title="MySQL" />
					<SiMongodb title="MongoDB" />
					<SiGraphql title="GraphQL" />
				</div>
			</div>
		</div>

		<!-- Decorative image 2 -->
		<div
			in:fly={{ y: 50, duration: 300, delay: 600 }}
			out:fly={{ y: 50, duration: 300 }}
			class="bg-main hidden items-center justify-center overflow-hidden rounded-3xl text-white/75 lg:col-span-2 lg:row-span-3 lg:flex"
		>
			<img src={shibuya} alt="Shibuya Crossing" class="h-full w-full object-cover" />
		</div>

		<!-- Main -->
		<div
			in:fade={{ duration: 500, delay: 600 }}
			out:fade={{ duration: 500 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-4 lg:row-span-2"
		>
			<h1 class="p-4 text-4xl font-semibold text-white">Kyle Shepherd</h1>
		</div>

		<!-- Education grid -->
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-4 lg:row-span-2"
		>
			<div class="flex flex-col gap-4 p-4">
				<div class="group">
					<h1 class="text-3xl font-semibold text-white">University of Tokyo</h1>
					<h2 class="mb-2 text-sm text-amber-300">Research Student</h2>
					<p class="text-lg">
						Post Graduate Research Student in the department of Information Science and Technology.
					</p>
				</div>
				<div class="group">
					<h1 class="text-3xl font-semibold text-white">University of the West Indies</h1>
					<h2 class="mb-2 text-sm text-amber-300">BSc. Computer Science</h2>
					<p class="text-lg">
						Graduated with First-Class Honours and a 3.99 GPA. Earned multiple scholarships and made
						the Dean's List.
					</p>
				</div>
			</div>
		</div>

		<!-- About grid -->
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-4 lg:row-span-1"
		>
			<div class="p-4">
				<h1 class="text-3xl font-semibold text-white">About Me</h1>
				<p class="">
					Passonate, motivated and adaptable is how I would describe myself. The greatest feeling
					one can experience is the accomplishment that comes from solving problems.
				</p>
				<!--  With code and just your imagination <span class="text-xs text-amber-300">&#40;and maybe a few libraries&#41;</span> anything is possible! -->
			</div>
		</div>
	</div>
</div>
