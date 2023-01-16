<script>
	export let data = {
		date: '',
		description: '',
		title: '',
		img: ''
	};
	const { date, img, title, description } = data;
</script>

<div class="blog-container">
	<span class="date">
		{date}
	</span>
	<img class="img" src={img} alt=""/>

	<span class="title">
		{title}
	</span>
	<span class="description">
		{description}
	</span>
</div>

<style>
	.blog-container {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		padding: 20px;
		gap: 12px;
		width: 346.67px;
		height: 410px;

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
		color: #787d8e;
	}
	.description {
		font-weight: 400;
		font-size: 14px;
		line-height: 24px;
		color: #787d8e;
	}
</style>
