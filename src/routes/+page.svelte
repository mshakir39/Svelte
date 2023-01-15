<script lang="ts">
	import Card from '../components/Card/index.svelte';
	import Navbar from '../components/Navbar/navbar.svelte';
	import Container from '../components/Container/container.svelte';
	import Hero from '../components/Hero/hero.svelte';
	import Brands from '../components/Brands/brands.svelte';
	import UniStoreSection from '../components/GenericSection/genericSection.svelte';
	import UniSearch from '../components/GenericSection/genericSection.svelte';


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
	<Hero />
	<Brands />
	<UniStoreSection
	features={["feature","feature","feature","feature","feature"]}
	Links={["LEARN MORE","AWS","GCP","AZURE"]}
		imgAlignLeft={false}
		img={'images/uniStore.svg'}
		h1={'store and manage data'}
		h2={' UniStore. World’s fastest <br> database.'}
		h3={'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'}
	/>
	<UniSearch
	features={["feature","feature","feature","feature","feature"]}
	Links={["LEARN MORE","AWS","GCP","AZURE"]}
		imgAlignLeft={true}
		img={'images/uniSearch.svg'}
		h1={'search something'}
		h2={' UniSearch. Future of Search.'}
		h3={'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'}
	/>
	<UniSearch
	features={["feature","feature","feature","feature","feature"]}
	Links={["LEARN MORE","AWS","GCP","AZURE"]}
		imgAlignLeft={false}
		img={'images/uniForm.svg'}
		h1={'ML something '}
		h2={' UniForm. Multi-Modal Encoder.'}
		h3={'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'}
	/>
</Container>

<style>
	:global(body) {
		font-family: 'Poppins';
	}
</style>
