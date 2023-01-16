<script>
	export let data = {
		date: '',
		description: '',
		title: '',
		img: ''
	};
	const { date, img, title, description } = data;
</script>

<div class="container">
	<span class="date">
		{date}
	</span>
	<div class="img" />

	<span class="title">
		{title}
	</span>
	<span class="description">
		{description}
	</span>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		padding: 20px;
		gap: 12px;
		width: 346.67px;
		height: 410px;
		background: #f7f9fc;
		margin-bottom: 54px;
	}
	.date {
		font-weight: 500;
		font-size: 14px;
		line-height: 21px;
		color: #b3b3b3;
	}
	.img {
		width: 306.67px;
		height: 200px;
		background: #d9d9d9;
	}
	.title {
		font-weight: 500;
		font-size: 18px;
		line-height: 27px;
		color: #000000;
	}
	.description {
		font-weight: 400;
		font-size: 14px;
		line-height: 21px;
		color: #787d8e;
	}
</style>
