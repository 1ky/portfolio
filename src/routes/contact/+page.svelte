<script>
	import { SiGithub } from "@icons-pack/svelte-simple-icons";
	import { SiProtonmail } from "@icons-pack/svelte-simple-icons";
</script>

<div class="flex justify-center w-full h-screen p-4">
    <div class="grid lg:grid-cols-4 lg:grid-rows-2 grid-flow-row-dense gap-4 w-full lg:max-w-[700px] h-full lg:max-h-[400px]">
        <div class="lg:col-span-2 lg:row-span-1 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center gap-1">
                <SiProtonmail title='Email' size={60} />
                <div class="bg-highlight rounded-3xl px-2">kyshepherd@protonmail.com</div>
            </div>
        </div>
        <div class="lg:col-span-2 lg:row-span-2 bg-main rounded-3xl flex justify-center items-center text-white/75">
            LinkedIn
        </div>
        <div class="lg:col-span-2 lg:row-span-1 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center gap-2">
                <SiGithub title='GitHub' size={60} />
                <div class="flex flex-col justify-center items-center">
                    <h2 class="text-sm text-white/50">1ky</h2>
                    <p class="text-xl">Check out my GitHub</p>
                </div>
            </div>
        </div>
    </div>   
</div>