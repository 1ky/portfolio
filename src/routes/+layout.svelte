<script lang="ts">
	import '../app.css';
	import { page } from '$app/state';

	let { children } = $props();
</script>

<nav class="fixed top-0 z-30 flex w-full justify-center bg-black/75 p-8 backdrop-blur-xs">
	<div class="bg-main flex items-center gap-4 rounded-xl p-2 font-semibold text-white/50">
		<a href="/"
			><div
				class={`rounded-lg px-2 py-1 ${page.route.id === '/' ? 'bg-highlight text-white' : ''}`}
			>
				Home
			</div></a
		>
		<a href="/projects"
			><div
				class={`rounded-lg px-2 py-1 ${page.route.id === '/projects' ? 'bg-highlight text-white' : ''}`}
			>
				Projects
			</div></a
		>
		<a href="/contact"
			><div
				class={`rounded-lg px-2 py-1 ${page.route.id === '/contact' ? 'bg-highlight text-white' : ''}`}
			>
				Contact
			</div></a
		>
	</div>
</nav>

{@render children()}
