<button class="button-style">
	<slot />
</button>

<style>
	.button-style {
		border: none;
		width: 179px;
		height: 40px;
		color: white;
		border-radius: 4px;
		background: #000000;
	}

	.button-style:hover {
		background: #31343f;
	}
	.button-style:focus {
		background: #787d8e;
	}
</style>
