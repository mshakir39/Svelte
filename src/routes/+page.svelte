<script lang="js">
	// import type {ISection} from 'src/Interfaces/Isections';
	import Card from '../components/Card/index.svelte';
	import Navbar from '../components/Navbar/navbar.svelte';
	import Container from '../components/Container/container.svelte';
	import Hero from '../components/Hero/hero.svelte';
	import Brands from '../components/Brands/brands.svelte';
	import Section from '../components/GenericSection/genericSection.svelte';
	import TechnologySection from '../components/TechnologySection/TechnologySection.svelte';
	import Contributions from '../components/Contributions/contributions.svelte';
	import BlogSection from '../components/BlogSection/blogSection.svelte';
	import Contact from "../components/Contact/contact.svelte"
	import Footer  from "../components/Footer/footer.svelte"

	const details = [
		{
			features: ['feature', 'feature', 'feature', 'feature', 'feature'],
			Links: ['LEARN MORE', 'AWS', 'GCP', 'AZURE'],
			imgAlignLeft: false,
			img: 'images/uniStore.svg',
			h1: 'store and manage data',
			h2: ' UniStore. World’s fastest <br> database.',
			h3: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'
		},
		{
			features: ['feature', 'feature', 'feature', 'feature', 'feature'],
			Links: ['LEARN MORE', 'AWS', 'GCP', 'AZURE'],
			imgAlignLeft: true,
			img: 'images/uniSearch.svg',
			h1: 'search something',
			h2: ' UniSearch. Future of Search.',
			h3: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'
		},
		{
			features: ['feature', 'feature', 'feature', 'feature', 'feature'],
			Links: ['LEARN MORE', 'AWS', 'GCP', 'AZURE'],
			imgAlignLeft: false,
			img: 'images/uniForm.svg',
			h1: 'ML something ',
			h2: '  UniForm. Multi-Modal Encoder.',
			h3: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'
		}
	] ;
</script>

<Navbar />
<Container>
	<Hero />
	<Brands />
	{#each details as detail } 
		<Section details={detail} />
	{/each}
	<TechnologySection />
	<Contributions />
	<BlogSection />
	<Contact/>

</Container>
<Footer/>
<style>
	:global(body) {
		font-family: 'Poppins';
	}
</style>
