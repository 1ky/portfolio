<script>
	import { SiArchlinux, SiCss3, SiGit, SiGithub, SiGraphql, SiHtml5, SiJavascript, SiMongodb, SiMysql, SiPython, SiReact, SiSvelte, SiTailwindcss, SiTypescript } from "@icons-pack/svelte-simple-icons";
    import shibuya from '$lib/assets/shibuya-crossing.jpg';
    import me from '$lib/assets/myself.jpg';
</script>

<div class="h-screen w-full flex justify-center items-center mb-10 p-4">
    <div class="grid grid-cols-1 lg:grid-cols-10 lg:grid-rows-4 grid-flow-row-dense h-full w-full lg:max-w-[1250px] gap-4">
        <!-- Github grid -->
        <div class="lg:col-span-2 lg:row-span- bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center gap-2">
                <SiGithub title='GitHub' size={60} />
                <div class="flex flex-col justify-center items-center">
                    <h2 class="text-sm text-white/50">github.com/1ky</h2>
                </div>
            </div>
        </div>

        <!-- Developer grid -->
        <div class="lg:col-span-4 lg:row-span-1 bg-amber-300/50 rounded-3xl flex justify-center items-center text-white/75">
            <h2 class="text-3xl font-semibold text-white p-4">Frontend/Full Stack Developer</h2>
        </div>

        <!-- Decorative image 1 -->
        <div class="lg:col-span-2 lg:row-span-2 bg-main rounded-3xl lg:flex justify-center items-center text-white/75 overflow-hidden hidden">
            <img src={me} alt="Kyle Shepherd" class="object-cover h-full w-full">
        </div>

        <!-- Specialties grid -->
        <div class="lg:col-span-2 lg:row-span-2 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col justify-center items-center">
                <h2 class="text-3xl font-semibold text-white p-4">Technologies</h2>
                <div class="flex flex-wrap gap-3 p-8 *:text-white/50 *:hover:text-white *:cursor-pointer">
                    <SiHtml5 title='HTML' />
                    <SiCss3 title='CSS' />
                    <SiJavascript title='JavaScript' />
                    <SiTypescript title='TypeScript' />
                    <SiPython title='Python' />
                    <SiReact title='React' />
                    <SiSvelte title='Svelte' />
                    <SiTailwindcss title='Tailwindcss' />
                    <SiGit title='Git' />
                    <SiArchlinux title='Arch Linux' />
                    <SiMysql title='MySQL' />
                    <SiMongodb title='MongoDB' />
                    <SiGraphql title='GraphQL' />
                </div>
            </div>
        </div>


        <!-- Decorative image 2 -->
        <div class="lg:col-span-2 lg:row-span-3 bg-main rounded-3xl lg:flex justify-center items-center text-white/75 overflow-hidden hidden">
            <img src={shibuya} alt="Shibuya Crossing" class="object-cover h-full w-full">
        </div>

        <!-- Main -->
        <div class="lg:col-span-4 lg:row-span-2 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <h1 class="text-4xl font-semibold text-white p-4">Kyle Shepherd</h1>
        </div>        
        
        <!-- Education grid -->
        <div class="lg:col-span-4 lg:row-span-2 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="flex flex-col gap-4 p-4">
                <div class="group">
                    <h1 class="text-3xl font-semibold text-white">University of Tokyo</h1>
                    <h2 class="text-sm text-amber-300 mb-2">Research Student</h2>
                    <p class="text-lg">Post Graduate Research Student in the department of Information Science and Technology.</p>
                </div>
                <div class="group">
                    <h1 class="text-3xl font-semibold text-white">University of the West Indies</h1>
                    <h2 class="text-sm text-amber-300 mb-2">BSc. Computer Science</h2>
                    <p class="text-lg">Graduated with First-Class Honours and a 3.99 GPA. Earned multiple scholarships and made the Dean's List.</p>
                </div>
            </div>
        </div>

        <!-- About grid -->
        <div class="lg:col-span-4 lg:row-span-1 bg-main rounded-3xl flex justify-center items-center text-white/75">
            <div class="p-4">
                <h1 class="text-3xl font-semibold text-white">About Me</h1>
                <p class="">Passonate, motivated and adaptable is how I would describe myself. The greatest feeling one can experience is the accomplishment that comes from solving problems.</p>
                <!--  With code and just your imagination <span class="text-xs text-amber-300">&#40;and maybe a few libraries&#41;</span> anything is possible! -->
            </div>
        </div>
    </div>
</div>