<script lang="ts">
	import '../app.css';
    import { page } from '$app/state';

	let { children } = $props();
</script>

<nav class="w-full flex justify-center p-8 fixed top-0 bg-white/75">
    <div class="bg-blue-300/75 text-white/75 font-semibold p-2 rounded-xl flex gap-4 items-center">
        <a href="/"><div class={`py-1 px-2 rounded-lg ${page.route.id === '/' ? 'bg-blue-700 text-white' : ''}`}>Home</div></a>
        <a href="/projects"><div class={`py-1 px-2 rounded-lg ${page.route.id === '/projects' ? 'bg-blue-700 text-white' : ''}`}>Projects</div></a>
        <a href="/contact"><div class={`py-1 px-2 rounded-lg ${page.route.id === '/contact' ? 'bg-blue-700 text-white' : ''}`}>Contact</div></a>
    </div>
</nav>

{@render children()}
