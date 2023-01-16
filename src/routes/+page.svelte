<script lang="ts">
	// import type {ISection} from 'src/Interfaces/Isections';
	import Card from '../components/Card/index.svelte';
	import Navbar from '../components/Navbar/navbar.svelte';
	import Container from '../components/Container/container.svelte';
	import Hero from '../components/Hero/hero.svelte';
	import Mission from '../components/Mission/mission.svelte';
	import Brands from '../components/Brands/brands.svelte';
	import Section from '../components/GenericSection/genericSection.svelte';
	import TechnologySection from '../components/TechnologySection/TechnologySection.svelte';
	import Contributions from '../components/Contributions/contributions.svelte';
	import BlogSection from '../components/BlogSection/blogSection.svelte';
	import Contact from '../components/Contact/contact.svelte';
	import Footer from '../components/Footer/footer.svelte';

	const details = [
		{
			features: ['– Any Data Format', '– Machine Learning Ready', '– Open Source and Enterprise Versions'],
			Links: ['LEARN MORE', 'AWS', 'GCP', 'AZURE'],
			imgAlignLeft: false,
			learnMore:true,
			comingSoon:false,
			img: 'images/uniStore.svg',
			h1: 'store and manage data',
			title1: ' UniStore',
			title2:"Fastest Transactional Database",
			h3: 'Our transactional persistent database can store media, tabular, document-like, network-like, or even vector data, combining unseen universality, with revolutionary speed.'
		},
		{
			features: ['– Real-time Semantic Search ', '– Hardware Accelerated', '– Non-metric Spaces ',],
			Links: ['LEARN MORE', 'AWS', 'GCP', 'AZURE'],
			imgAlignLeft: true,
			learnMore:false,
			comingSoon:true,
			img: 'images/uniSearch.svg',
			h1: 'search something',
			title1: ' UniStore',
			title2:"Fastest Transactional Database",
			h3: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'
		},
		{
			features: ['– Multi-Lingual ', '– Multi-Modal Transformers', '– Light Weight '],
			Links: ['LEARN MORE', 'AWS', 'GCP', 'AZURE'],
			imgAlignLeft: false,
			learnMore:false,
			comingSoon:true,
			img: 'images/uniForm.svg',
			h1: 'ML something ',
			title1: ' UniStore',
			title2:"Fastest Transactional Database",
			h3: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis. tech behind UKV'
		}
	];
</script>

<Navbar />
<Container>
	<Hero />
	<Mission />
	<Brands />
	<div class="ourProducts">Our Products</div>
	{#each details as detail}
		<Section details={detail} />
	{/each}
	<TechnologySection />
	<Contributions />
	<BlogSection />
	<Contact />
</Container>
<Footer />

<style>
	:global(body) {
		font-family: 'Poppins';
	}
	.ourProducts {
		width: 1077px;
		height: 45px;
		margin-bottom: 70px;
		font-family: 'Poppins';
		font-style: normal;
		font-weight: 500;
		font-size: 32px;
		line-height: 48px;
		text-align: center;
		color: #31343f;
	}
</style>
