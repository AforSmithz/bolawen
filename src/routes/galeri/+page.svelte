<script>
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
	// Default theme
	import '@splidejs/svelte-splide/css';

	import Batik from '$lib/images/batik.png';
	import HomeImg from '$lib/images/home-foto.png';
</script>

<svelte:head>
	<title>Home | Dusun Bolawen</title>
	<meta name="description" content="Website profile dusun Bolawen" />
</svelte:head>

<section
	class="relative pt-5 flex items-center flex-wrap-reverse justify-center bg-[#EEEBE3] h-screen z-[-999] gap-20"
>
	<img
		class="absolute left-[50%] top-[50%] translate-x-[-50%] translate-y-[-50%] z-[-1] h-[40rem]"
		src={Batik}
		alt="Welcome"
	/>
	<div class="flex gap-5 flex-col w-[35rem]">
		<div class="text-5xl font-extrabold">BOLAWEN</div>
		<Splide aria-label="My Favorite Images">
			{#each { length: 16 } as _, i}
				<SplideSlide>
					<img class="h-[20rem]" src={HomeImg} />
				</SplideSlide>
			{/each}
		</Splide>
	</div>
</section>
