<script>
	import Contributors from '../../components/Card/index.svelte';
	const details  = [
		{
			title: 'Universal key value',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB • UMem • UDisk × from C • C++ • Python • Java • GoLang',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 5
		},
		{
			title: 'Universal key value',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB • UMem • UDisk × from C • C++ • Python • Java • GoLang',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 5
		},
		{
			title: 'Universal key value',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB • UMem • UDisk × from C • C++ • Python • Java • GoLang',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 5
		},
		{
			title: 'Universal key value',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB • UMem • UDisk × from C • C++ • Python • Java • GoLang',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 5
		}
	] ;
</script>

<div class="parent">
	<div class="text-area">
		<span class="h1"> ML something </span>
		<span class="h2">Open source contributions</span>
		<span class="h3"
			>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
			labore et dolore magna aliqua. Ut enim ad minim
		</span>
	</div>
	<div style="display:flex;flex-wrap: wrap;">
		{#each details as detail}
			<div style="flex:50%">
				<Contributors details={detail} />
			</div>
		{/each}
	</div>
</div>

<style>
	.parent {
		display: flex;
		flex-direction: column;
        margin-bottom: 200px;
	}
	.text-area {
		display: flex;
		flex-direction: column;
		width: 550px;

		/* width: 453px; */
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
		margin-bottom: 40px;
	}
</style>
