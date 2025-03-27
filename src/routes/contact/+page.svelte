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
				<SiProtonmail title="Email" size={60} />
				<div class="bg-highlight rounded-3xl px-2">kyshepherd@protonmail.com</div>
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
				<SiInvision title="LinkedIn" size={60} />
				<div class=" rounded-3xl px-2">linkedin.com/in/1ky</div>
			</div>
		</div>
		<div
			in:fly={{ x: -50, duration: 300, delay: 600 }}
			out:fly={{ x: -50, duration: 300 }}
			class="bg-main flex items-center justify-center rounded-3xl text-white/75 lg:col-span-2 lg:row-span-1"
		>
			<div class="flex flex-col items-center justify-center gap-2">
				<div class="flex cursor-pointer flex-col items-center justify-center hover:text-white">
					<SiGithub title="GitHub" size={60} />
					<h2 class="text-sm text-white/50">github.com/1ky</h2>
				</div>
				<div class="">
					<p class="text-xl">Check out my GitHub</p>
				</div>
			</div>
		</div>
	</div>
</div>
