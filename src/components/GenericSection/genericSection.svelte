<script lang="ts">
	// import type { ISection } from '../../Interfaces/Isections.js';
	export let details = {
		h1: '',
		title1: '',
		title2: '',
		h3: '',
		img: '',
		comingSoon:false,
		imgAlignLeft: false,
		learnMore: false,
		features: [''],
		Links: ['']
	};

	let margin = '';

	const { h1, title1, title2, h3, img, imgAlignLeft, features, Links, learnMore,comingSoon } = details;
	if (learnMore === false) {
		margin = '12%';
	}
</script>

<div
	class="main-container "
	style={`flex-direction:${imgAlignLeft === true ? 'row-reverse' : 'row'}`}
>
	<div class="text-area">
		{#if comingSoon===true}
		<div class="coming-soon">Coming Soon</div>
		{/if}
		<!-- <span class="h1"> {h1}</span> -->
		<span />
		<span class="h2">{title1}</span>
		<span class="title2">{title2}</span>
		<span class="h3"> {h3}</span>
		<div class="features" style="margin-top:{margin}">
			{#each features as feature}
				<span style="margin-bottom:8px">{feature}</span>
			{/each}
		</div>
		<div class="links">
			{#if learnMore === true}
				<span style="margin-right:22px">learn more</span>
				<img src="images/smallAws.svg" alt="aws" style="margin-right:22px" />
				<img src="images/smallGc.svg" alt="gc" style="margin-right:22px" />
				<img src="images/Learnmore3.svg" alt="aws" />
			{/if}
		</div>
	</div>
	<img src={img} alt="" />
</div>

<style>
	.main-container {
		display: flex;
		margin-bottom: 200px;
	}
	.coming-soon{
		width: 111px;
height: 22px;
text-align: center;
font-size: 14px;
font-weight: 500;
background: #F2F4FB;
border-radius: 4px;
margin-bottom: 29px;
color: #787D8E;
	}
	.features {
		font-weight: 500;
		display: flex;
		flex-direction: column;
		font-size: 16px;
		line-height: 24px;

		color: #000000;
	}
	.links {
		display: flex;
		margin-top: 43px;
		text-transform: uppercase;
		font-weight: 500;
		font-size: 14px;
		line-height: 18px;
		color: #787d8e;
	}
	.text-area {
		display: flex;
		flex-direction: column;
		width: 453px;
	}
	.title2 {
		font-style: normal;
		font-weight: 300;
		font-size: 28px;
		line-height: 38px;
		margin-bottom: 12px;
	}
	/* .h1 {
		margin-top: 24px;
		font-weight: 500;
		font-size: 12px;
		line-height: 18px;
		color: #b3b3b3;
	} */
	.h2 {
		margin-bottom: 0;
		font-weight: 500;
		font-size: 28px;
		line-height: 42px;
		color: black;
	}
	.h3 {
		width: 453px;
		height: 72px;
		margin-bottom: 24px;
		font-family: 'Poppins';
		font-style: normal;
		font-weight: 400;
		font-size: 14px;
		line-height: 24px;

		color: #787d8e;
	}

	@media (max-width: 767px) {
		.main-container {
			flex-direction: column !important;
			justify-content: center;
			align-items: center;
			display: flex;
		}
		.text-area {
			display: flex;
			flex-direction: column;
			width: 453px;
			align-items: center;
		}
	}
</style>
