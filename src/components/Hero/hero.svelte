<script>
	import Button from '../Button/button.svelte';
</script>

<div class="parent">
	<img src="/images/heroLogo.svg" alt="Unum" />
	<div class="inner-container">
		<img
			src="/images/brandLogoBlack.svg"
			alt="Unum"
			height="32"
			width="32"
			style="margin-bottom:36px"
		/>
		<span class="heading"> Unum. Scaling Intelligence. </span>
		<span class="des">
			Building Core Technologies for Data-Lakes <br /> and Cloud Providers.
		</span>
		<div style="display:flex">
			<Button>CONTACT SALES</Button>
			<span class="docs"> Read the Docs</span>
		</div>
	</div>
</div>

<style>
	.parent {
		display: flex;
		height: 560px;
		justify-content: space-between;
		align-items: center;
		margin-top: 5%;
		margin-right: 120px;
	}
	.inner-container {
		display: flex;
		flex-direction: column;
	}
	.heading {
		font-weight: 500;
		font-size: 28px;
		line-height: 42px;
	}
	.des {
		font-weight: 500;
		font-size: 18px;
		line-height: 27px;
		color: #787d8e;
		margin-bottom: 45px;
	}
	.docs {
		font-style: normal;
		font-weight: 500;
		font-size: 14px;
		line-height: 18px;
		text-transform: uppercase;
		color: #787d8e;
		margin-left: 32px;
		display: flex;
		align-items: center;
	}
	.docs:hover {
		color: black;
	}
	@media (max-width: 767px) {
		.parent {
			display: flex;
			flex-direction: column;
			margin-right: 0;
		}
		.inner-container {
			align-items: center;
			margin-top: 53px;
		}
	}
</style>
