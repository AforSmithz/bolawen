<script lang="ts">
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
	import type { stringify } from 'postcss';

	const fontColor: { [key: string]: string } = {
		'/tentang': 'text-white',
		'/geografis': 'text-black',
		'/pemerintah': 'text-white',
		'/kontak': 'text-white'
	};
</script>

<header class="bg-[#EEEBE3] absolute w-screen bg-transparent">
	<nav
		class={`flex items-center justify-center gap-12 p-5 font-bold ${fontColor[$page.url.pathname]}`}
	>
		<div aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
			<a href="/">HOME</a>
		</div>
		<div aria-current={$page.url.pathname === '/tentang' ? 'page' : undefined}>
			<a href="/tentang">TENTANG DESA</a>
		</div>
		<div aria-current={$page.url.pathname === '/geografis' ? 'page' : undefined}>
			<a href="/geografis">GEOGRAFIS DESA</a>
		</div>
		<!-- <div aria-current={$page.url.pathname.startsWith('/pemerintah') ? 'page' : undefined}>
			<a href="/pemerintah">PEMERINTAH</a>
		</div> -->
		<div aria-current={$page.url.pathname.startsWith('/galeri') ? 'page' : undefined}>
			<a href="/galeri">GALERI</a>
		</div>
	</nav>
</header>
