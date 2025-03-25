<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<nav class="w-full flex justify-center p-8 fixed top-0">
    <div class="bg-blue-500 text-white p-2 rounded-xl flex gap-4 items-center">
        <a href="/"><div class="py-1 px-2 bg-blue-300 rounded-lg">Home</div></a>
        <a href="/projects"><div class="py-1 px-2 rounded-lg">Projects</div></a>
        <a href="/contact"><div class="py-1 px-2 rounded-lg">Contact</div></a>
    </div>
</nav>

{@render children()}
