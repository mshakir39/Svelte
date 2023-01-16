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
	<span class="h1"> ML something </span>
	<span class="h2">Technology behind</span>
	<span class="h3"
		>Unum covers every step of the modern Data Processing – from Storage to in-<br />built ML and
		modelling</span
	>
	<div class="parent">
		{#each technologies as tech}
			<div class="techParent">
				<span class="tech">
					{tech.name}
				</span>
				<img src={tech.imgSrc} alt="" />
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
    .parent{
        display:flex;
        justify-content: space-around;
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
		margin-top: 4px;
		font-weight: 500;
		font-size: 28px;
		line-height: 42px;
		color: black;
	}
	.h3 {
		font-weight: 500;
		font-size: 14px;
		line-height: 21px;
		color: #b3b3b3;
		margin-bottom: 56px;
	}
	.feat {
		font-size: 18px;
		line-height: 27px;
		font-weight: 500;
		margin-top: 16px;
		text-align: center;
	}
	.tech {
		font-size: 16px;
		line-height: 24px;
		text-align: center;
		color: #787d8e;
		margin-bottom: 16px;
	}
</style>
