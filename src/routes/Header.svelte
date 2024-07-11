<script>
	import { page } from '$app/stores';
</script>

<header class="w-full bg-[#4A4A5A] text-white py-16 text-lg ">

	<section class="mb-14 w-full flex justify-center">
		<div class="w-1/2 flex h-80 space-x-6">
	
			<img src="kishmat_bhattarai.jpeg" class="object-contain" alt="kishmat">
	
			<div class="flex flex-col h-full w-full space-y-5 ">
				<h1 class="h-1/6 text-3xl text-yellow-200">
					Kishmat Bhattarai
				</h1>
	
				<div class="h-5/6 flex flex-col p-4 bg-[#2E2D3C] space-y-2">
					<div class="font-extralight">Undergraduate Bachelor of Computer Science</div>
					<div class="font-light">
						Software Developer | Python, Web, ML, NLP
						<p>Kathmandu, Nepal</p>
						<p>kishmat17@gmail.com</p>
					</div>
				</div>
			</div>
	
		</div>
	</section>

	<nav class="bg-[#2E2D3C] ml-52 ">
		<ul class="flex justify-center text-2xl space-x-4 h-16 items-center">
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/projects') ? 'page' : undefined}>
				<a href="/projects">Projects</a>
			</li>
		</ul>
	</nav>
</header>

