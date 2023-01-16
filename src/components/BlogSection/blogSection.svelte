<script>
	import Blog from '../Blog/blog.svelte';
	const data = [
		{
			date: 'Nov 30,2022',
			img: 'images/blog1.png',
			title: 'Pandas, CuDF, Modin, Arrow, Spark, and a Billion Taxi Rides',
			description:
				'Choosing the right in-memory tabular processing framework'
		},
		{
			date: 'Nov 30,2022',
			img: 'images/blog2.png',
			title: '879 GB/s Parallel Reductions in C++ and CUDA',
			description:
				'Pushing the limits of memory-bound tasks on DDR4-powered CPUs and GDDR6-powered GPUs'
		},
		{
			date: 'Nov 30,2022',
			img: 'images/blog3.png',
			title: 'CuPy = 50x Faster NumPy',
			description:
				'Finding the easiest ways to accelerate your Linear Algebra workloads on modern GPUs'
		},
	
	];
</script>

<div class="blog-container">
	<!-- <span class="h1"> ML something </span> -->
	<span class="h2">Top Technical Articles from our Blog</span>
	<div class="blog-parent">
		{#each data as detail}
			<div style="flex:33%">
				<Blog data={detail} />
			</div>
		{/each}
	</div>
</div>

<style>
	.blog-container {
		display: flex;
		flex-direction: column;
		/* align-items: center; */
		padding: 41px 0px;
		margin-bottom: 194px;
	}
	.blog-parent {
		display: flex;
		flex-wrap: wrap;
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
		margin-bottom: 52px;
		font-weight: 500;
		font-size: 28px;
		line-height: 42px;
		color: black;
	}
	@media (max-width: 767px) {
		.blog-parent {
			display: flex;
			flex-wrap: wrap;
			flex-direction: column;
		}
		.blog-container {
			align-items: center;
		}
	}
</style>
