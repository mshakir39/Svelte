<div class="main-container">
	<slot />
</div>

<style>
	.main-container {
		margin-right: 160px;
		margin-left: 160px;
	}
	@media (max-width: 767px) {
		.main-container {
			margin-right: 0;
			margin-left: 0;
		}
	}
</style>
