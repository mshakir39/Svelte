<div class="brands">
	<img src="images/brand1.svg" alt="nvdia" />
	<img src="images/brand2.svg" alt="amazon" />
	<img src="images/brand3.svg" alt="git" />
	<img src="images/brand4.svg" alt="infinity" />
</div>

<style>
	.brands {
		display: flex;
		justify-content: space-around;
		margin-top: 200px;
		margin-bottom: 200px;
	}
	@media (max-width: 767px) {
		.brands {
			flex-direction: column;
			display: flex;
			margin-top: 432px;
			gap: 67px;
			justify-content: center;
			align-items: center;
		}
	}
</style>
