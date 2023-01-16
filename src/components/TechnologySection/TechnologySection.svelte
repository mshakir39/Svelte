<script>
	const technologies = [
		{
			name: 'NETWORKING',
			imgSrc: '/images/tech1.svg',
			technology: 'UJPRC'
		},
		{
			name: 'SEARCH',
			imgSrc: '/images/tech2.svg',
			technology: 'UniSearch'
		},
		{
			name: 'SEARCH',
			imgSrc: '/images/tech3.svg',
			technology: 'UniSearch'
		},
		{
			name: 'ENCODER',
			imgSrc: '/images/tech4.svg',
			technology: 'UniForm'
		},
		{
			name: 'ML',
			imgSrc: '/images/tech5.svg',
			technology: 'UML'
		}
	];
</script>

<div class="text-area">
	<!-- <span class="h1"> ML something </span> -->
	<span class="h2">Technology behind</span>
	<span class="h3"
		>For every of our products we created custom tech for storage, networking,<br /> compute, or AI modelling</span
	>
	<div class="parent">
		{#each technologies as tech}
			<div class="techParent">
				<span class="tech">
					{tech.name}
				</span>
				<img src={tech.imgSrc} alt="technologies" />
				<span class="feat"> {tech.technology}</span>
			</div>
		{/each}
	</div>
</div>

<style>
	.text-area {
		display: flex;
		flex-direction: column;
		margin-bottom: 200px;

		/* width: 453px; */
	}
	.parent {
		display: flex;
		justify-content: space-between;
	}
	.techParent {
		display: flex;
		flex-direction: column;
	}
	.h1 {
		margin-top: 24px;
		font-weight: 500;
		font-size: 12px;
		line-height: 18px;
		color: #b3b3b3;
	}
	.h2 {
		margin-bottom: 12px;
		font-weight: 500;
		font-size: 28px;
		line-height: 42px;
		color: black;
	}
	.h3 {
		font-weight: 500;
		font-size: 14px;
		line-height: 21px;
		color: #787d8e;
		margin-bottom: 76px;
	}
	.feat {
		font-weight: 500;
		font-size: 18px;
		line-height: 27px;
		color: #787d8e;
		margin-top: 22px;
		text-align: center;
	}
	.tech {
		font-weight: 500;
		font-size: 14px;
		line-height: 18px;
		text-align: center;
		color: #787d8e;
		margin-bottom: 16px;
	}

	@media (max-width: 767px) {
		.text-area {
			align-items: center;
		}
		.parent {
			display: flex;
			width: auto;
			flex-direction: column;
			justify-content: center;
			align-items: center;
		}

		.techParent {
			display: flex;
			flex-direction: column;
			width: fit-content;
		}
	}
</style>
