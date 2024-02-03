<script>
	import Batik from '$lib/images/batik.png';
	import HomeImg from '$lib/images/home-foto.png';
</script>

<svelte:head>
	<title>Struktur Pemerintah | Dusun Bolawen</title>
	<meta name="description" content="Sejarah dusun Bolawen" />
</svelte:head>

<section
	class="relative overflow-hidden pt-5 flex items-center flex-wrap-reverse justify-center bg-[#083522] h-screen z-[-999] gap-20"
>
	<img class="absolute right-[2%] top-[-5%] z-[-1] h-[29rem]" src={Batik} alt="Welcome" />
	<img
		class="overflow-hidden absolute left-[2%] bottom-[-20%] z-[-1] h-[29rem]"
		src={Batik}
		alt="Welcome"
	/>
	<div class="flex gap-5 flex-col w-[35rem]">
		<div class="text-5xl font-extrabold text-white">Struktur Pemerintah</div>
		<div class="text-white">
			Dusun Bolawen, terletak di Kabupaten Sleman, memiliki sejarah kaya yang melibatkan tokoh-tokoh
			penting seperti Kyai Baulawi. Kyai Baulawi, awalnya dikenal sebagai Kyai Abdulhadi
			Prawirokusumo, merupakan seorang ulama dan penasihat spiritual Pangeran Diponegoro. Nama
			"Baulawi" berasal dari "Mbulawi" atau "mambu lawe," yang mengindikasikan orang yang sudah tua
			dan mendekati kematian. Kyai Baulawi tiba di Bolawen setelah kejar-kejaran dengan pasukan
			Belanda, membawa peninggalan berupa Al Qur'an yang kini disimpan di pesantren. Dia juga
			memiliki peran penting dalam mengalihkan aliran sungai Bedhog untuk melindungi penduduk dari
			banjir. Kyai Baulawi mendirikan masjid dan meninggal pada 1833, dikebumikan di makam Padukuhan
			Bolawen, di mana setiap tahun diadakan peringatan Haul pada tanggal 2 Sya'ban.
		</div>
	</div>
	<!-- <img class="h-[35rem]" src={HomeImg} /> -->
</section>
