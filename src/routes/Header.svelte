<script>
	import { page } from '$app/stores';
</script>

<header class="w-full bg-gray-600 text-white py-16 ">

	<section class="mb-14 w-full flex justify-center">
		<div class="w-1/2 flex h-72 space-x-6">
	
			<img src="kishmat_bhattarai.jpeg" class="object-contain" alt="kishmat">
	
			<div class="flex flex-col h-full w-full space-y-5 ">
				<h1 class="h-1/6 text-xl">
					Kishmat Bhattarai
				</h1>
	
				<div class="h-5/6 flex flex-col p-4 bg-gray-700 space-y-2">
					<div>Undergraduate Bachelor of Computer Science</div>
					<div>Software Developer | Python, Web, ML, NLP</div>
				</div>
			</div>
	
		</div>
	</section>

	<nav class="bg-gray-700 ">
		<ul class="flex justify-center text-lg space-x-4 h-14 items-center">
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

