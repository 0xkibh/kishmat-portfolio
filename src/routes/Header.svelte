<script>
	import { base } from '$app/paths';
	import { page } from '$app/stores';

	let menuOpen = true;

	let menuToogle = () => {
		console.log(menuOpen)
		menuOpen = !menuOpen
	}
</script>

<style>
    .menu-hidden {
        display: none;
    }
</style>

<header class="w-full bg-[#4A4A5A] text-white {menuOpen ? 'py-10' : 'pt-10 pb-2'} md:py-16 text-lg">
    <section class="py-3 md:mb-14 w-full flex justify-center">
        <div class="w-full md:w-1/2 flex flex-col md:flex-row h-auto md:h-80 space-x-0 md:space-x-6">
            <img src="kishmat_bhattarai.jpeg" class="object-contain h-40 md:h-full mx-auto md:mx-0" alt="kishmat">
            <div class="flex flex-col h-full w-full space-y-5 p-4 md:p-0">
                <h1 class="text-2xl md:text-3xl text-yellow-200">
                    Kishmat Bhattarai
                </h1>
                <div class="h-full flex flex-col p-4 bg-[#2E2D3C] space-y-2">
                    <div class="font-extralight">Undergraduate Bachelor of Computer Science</div>
                    <div class="font-light">
                        Software Developer | Python, Web, ML, NLP
                        <p>Kathmandu, Nepal</p>
                        <a href="mailto:kishmat17@gmail.com" class="underline">kishmat17@gmail.com</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <nav class="md:bg-[#2E2D3C] relative md:ml-40">
		<div class="md:hidden flex justify-end p-4">
            <button on:click={menuToogle} class="text-white focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
                </svg>
            </button>
        </div>
        <ul class="flex flex-col md:flex-row md:pl-40 text-xl md:text-2xl space-y-6 md:space-y-0 md:space-x-4 h-auto md:h-16 items-center" class:menu-hidden={!menuOpen}>
            <li aria-current={$page.url.pathname === base + '/' ? 'page' : undefined}>
                <a href="{base}">Home</a>
            </li>
            <li aria-current={$page.url.pathname === base + '/about' ? 'page' : undefined}>
                <a href="{base}/about">About</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith(base + '/projects') ? 'page' : undefined}>
                <a href="{base}/projects">Projects</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith(base + '/blogs') ? 'page' : undefined}>
                <a href="{base}/blogs">Blogs</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith(base + '/cv') ? 'page' : undefined}>
                <a href="{base}/kishmat_cv.pdf" target="_blank">CV</a>
            </li>
        </ul>
    </nav>
</header>

