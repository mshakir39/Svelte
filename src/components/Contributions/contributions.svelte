<script>
	import Contributors from '../../components/Card/index.svelte';
	const details = [
		{
			title: 'Universal Keys & Values',
			description:
				'Universal DBMS for Docs • Graphs • Blobs • Vectors × in Local • Remote × RocksDB • LevelDB • UMem • UDisk × from C • C++ • Python • Java • GoLang',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 4
		},
		{
			title: 'Unexceptionally Consistent Set',
			description:
				'If only std::set was a DBMS: collection of templated ACID in-memory exception-free thread-safe and concurrent containers in a header-only library',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 4
		},
		{
			title: 'Uncluttered Navigable Small Worlds',
			description:
				'Tiny Approximate Nearest Neighbors Search library for large point clouds in not necceserily metric spaces, with online updates, and hardware acceleration with x86 AVX2, AVX-512, and Arm Neon',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 4
		},
		{
			title: 'Uninterrupted JSON Remote Procedure Calls',
			description:
				'Remember FastAPI? This is 100x Fast-ER-API, implementing JSON-RPC, and based on interrupt-less IO technologies, like io_uring, and wrapped into a familiar Python interface',
			status: 'public',
			lang: 'C++',
			stars: 64,
			shares: 4
		}
	];
</script>

<div class="parent">
	<div class="text-area">
		<!-- <span class="h1"> ML something </span> -->
		<span class="h2">Open source contributions</span>
		<span class="h3">Our team created and is Maintaining the following Repositories. </span>
	</div>
	<div class="contributer-parent">
		{#each details as detail}
			<div style="flex:50%">
				<Contributors details={detail} />
			</div>
		{/each}
	</div>
</div>

<style>
	.contributer-parent {
		display: flex;
		flex-wrap: wrap;
	}
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

	/* .h1 {
		margin-top: 24px;
		font-weight: 500;
		font-size: 12px;
		line-height: 18px;
		color: #b3b3b3;
	} */
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
		color: #787d8e;
		margin-bottom: 40px;
	}
	@media (max-width: 767px) {
		.contributer-parent {
			display: flex;
			flex-wrap: wrap;
			flex-direction: column;
		}
		.parent {
			align-items: center;
		}
	}
</style>
