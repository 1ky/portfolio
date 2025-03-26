<script>
	import { SiGithub, SiProtonmail, SiInvision } from "@icons-pack/svelte-simple-icons";
</script>

<div class="flex justify-center w-full h-screen p-4">
    <div class="grid lg:grid-cols-4 lg:grid-rows-2 grid-flow-row-dense gap-4 w-full lg:max-w-[700px] h-full lg:max-h-[400px]">
        <div class="lg:col-span-2 lg:row-span-1 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center gap-1 *:cursor-pointer *:hover:text-white">
                <SiProtonmail title='Email' size={60} />
                <div class="bg-highlight rounded-3xl px-2">kyshepherd@protonmail.com</div>
            </div>
        </div>
        <div class="lg:col-span-2 lg:row-span-2 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center gap-1 *:cursor-pointer *:hover:text-white">
                <SiInvision title='LinkedIn' size={60} />
                <div class=" rounded-3xl px-2">linkedin.com/in/1ky</div>
            </div>          
        </div>
        <div class="lg:col-span-2 lg:row-span-1 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center gap-2">
                <div class="flex flex-col justify-center items-center cursor-pointer hover:text-white">
                    <SiGithub title='GitHub' size={60} />
                    <h2 class="text-sm text-white/50">github.com/1ky</h2>
                </div>
                <div class="">
                    <p class="text-xl">Check out my GitHub</p>
                </div>
            </div>
        </div>
    </div>   
</div>