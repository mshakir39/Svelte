<script lang="ts">
	import Card from '../components/Card/index.svelte';
	import Navbar from '../components/Navbar/navbar.svelte';
	import Container from '../components/Container/container.svelte';
	import Hero from '../components/Hero/hero.svelte';
import Brands from "../components/Brands/brands.svelte"


	// const details = {
	// 	title: 'Universal key value',
	// 	description:
	// 		'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB • UMem • UDisk × from C • C++ • Python • Java • GoLang',
	// 	status: 'public',
	// 	lang: 'C++',
	// 	stars: 64,
	// 	shares: 5
	// };
</script>

	<Navbar />
	<Container>
	<Hero/>
	<Brands/>
	</Container>




<style >
	:global(body){

		font-family: 'Poppins'
	
	}
</style>