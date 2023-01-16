<script>
	import Blog from '../Blog/blog.svelte';
	const data = [
		{
			date: 'Nov 30,2022',
			img: '',
			title: 'Powering Next Generation Applications with UniStore ',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB '
		},
		{
			date: 'Nov 30,2022',
			img: '',
			title: 'Powering Next Generation Applications with UniStore ',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB '
		},
		{
			date: 'Nov 30,2022',
			img: '',
			title: 'Powering Next Generation Applications with UniStore ',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB '
		},
		{
			date: 'Nov 30,2022',
			img: '',
			title: 'Powering Next Generation Applications with UniStore ',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB '
		}
	];
</script>

<div class="blog-container">
	<span class="h1"> ML something </span>
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
