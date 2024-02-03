<script>
	import { Button, Modal } from 'flowbite-svelte';
	import tilt from 'svelte-tilt';
	import Batik from '$lib/images/batik.png';
	import Administrasi from '$lib/images/administrasi.jpg';
	import Lahan from '$lib/images/penutupan-lahan.jpg';
	import TPS from '$lib/images/tps.jpg';
	import Evakuasi from '$lib/images/jalur-evakuasi.jpg';

	let isModal = false;
	const maps = [
		{ img: Administrasi, isOpen: false },
		{ img: Lahan, isOpen: false },
		{ img: TPS, isOpen: false },
		{ img: Evakuasi, isOpen: false }
	];
</script>

<svelte:head>
	<title>Geografis Dusun | Dusun Bolawen</title>
	<meta name="description" content="Sejarah dusun Bolawen" />
</svelte:head>

<section
	class="overflow-hidden pt-5 flex-col flex items-center justify-center bg-[#EEEBE3] h-screen z-[-999] gap-5"
>
	<img class="absolute right-[2%] bottom-[-20%] h-[29rem]" src={Batik} alt="Welcome" />
	<img class="absolute left-[2%] top-[-5%] h-[29rem]" src={Batik} alt="Welcome" />
	<div class="text-5xl font-extrabold">Geografis Dusun</div>
	<div class="flex flex-wrap gap-5 items-center justify-center">
		{#each maps as { img, isOpen }}
			<img
				on:click={() => (isOpen = true)}
				use:tilt={{ reverse: true, scale: 1.2 }}
				class="h-[19rem]"
				src={img}
			/>
		{/each}
	</div>
</section>

{#each maps as { img, isOpen }}
	<Modal size={img === Administrasi ? 'md' : 'xl'} bind:open={isOpen} autoclose outsideclose>
		<div class="flex items-center justify-center">
			<img class="h-[45rem]" src={img} />
		</div>
	</Modal>
{/each}
