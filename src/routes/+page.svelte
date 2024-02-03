<script>
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
		<div>
			Dalam Dusun Bolawen, harmoni antara umat beragama terlihat dalam perbandingan jumlah penduduk
			yang cukup seimbang antara penganut agama Katolik dan Islam. Meskipun cikal bakal nama Bolawen
			berasal dari seorang ulama Islam, Kyai Baulawi, yang pernah tinggal di sana, sejarah mencatat
			bahwa pada suatu masa, penganut agama Katolik menjadi mayoritas. Meski demikian, kondisi ini
			tidak memengaruhi persatuan masyarakat, dan melalui waktu, terjadi perubahan dinamika yang
			membawa kedamaian dan kerukunan antarumat beragama. Kegiatan bersama, seperti pembangunan
			masjid dan kegiatan sosial, mencerminkan semangat toleransi dan saling menghormati antarumat
			beragama di Dusun Bolawen.
		</div>
	</div>
	<img class="h-[35rem]" src={HomeImg} />
</section>
