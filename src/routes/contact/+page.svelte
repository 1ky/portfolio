<script>
	import { fly } from 'svelte/transition';
	import { SiGithub, SiProtonmail, SiInvision } from '@icons-pack/svelte-simple-icons';
</script>

<div class="flex h-screen w-full justify-center p-4">
	<div
		class="grid h-full w-full grid-flow-row-dense gap-4 lg:max-h-[400px] lg:max-w-[700px] lg:grid-cols-4 lg:grid-rows-2"
	>
		<div
			in:fly={{ x: -50, duration: 300, delay: 600 }}
			out:fly={{ x: -50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-2 lg:row-span-1"
		>
			<div
				class="flex flex-col items-center justify-center gap-1 *:cursor-pointer *:hover:text-white"
			>
				<a href="mailto:kyshepherd@protonmail.com">
					<SiProtonmail title="Email" size={60} />
				</a>
				<a href="mailto:kyshepherd@protonmail.com">
					<div class="bg-highlight rounded-3xl px-2">kyshepherd@protonmail.com</div>
				</a>
			</div>
		</div>
		<div
			in:fly={{ x: 50, duration: 300, delay: 600 }}
			out:fly={{ x: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-2 lg:row-span-2"
		>
			<div
				class="flex flex-col items-center justify-center gap-1 *:cursor-pointer *:hover:text-white"
			>
				<a href="https://www.linkedin.com/in/1ky/">
					<SiInvision title="LinkedIn" size={60} />
				</a>
				<a href="https://www.linkedin.com/in/1ky/">
					<div class=" rounded-3xl px-2">linkedin.com/in/1ky</div>
				</a>
			</div>
		</div>
		<div
			in:fly={{ y: 50, duration: 300, delay: 600 }}
			out:fly={{ y: 50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-2 lg:row-span-1"
		>
			<div class="flex flex-col items-center justify-center gap-2">
				<div class="flex cursor-pointer flex-col items-center justify-center hover:text-white">
					<a href="https://github.com/1ky">
						<SiGithub title="GitHub" size={60} />
					</a>
					<h2 class="text-sm text-white/50">github.com/1ky</h2>
				</div>
				<div class="">
					<p class="text-xl">Check out my GitHub</p>
				</div>
			</div>
		</div>
	</div>
</div>
