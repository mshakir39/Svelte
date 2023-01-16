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
		},{
			date: 'Nov 30,2022',
			img: '',
			title: 'Powering Next Generation Applications with UniStore ',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB '
		}
	];
</script>

<div class="container">
    <span class="h1"> ML something </span>
		<span class="h2">Top Technical Articles from our Blog</span>
    <div style="display:flex;flex-wrap: wrap;">
	{#each data as detail}
		<div style="flex:33%">
			<Blog data={detail} />
		</div>
	{/each}
    </div>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		/* align-items: center; */
		padding: 41px 0px;
        margin-bottom: 194px;
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
</style>
