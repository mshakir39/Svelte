<div class="contact-container">
	<span class="work">Lets Work Together!</span>
	<input type="text" class="input" placeholder="Your email"/>
	<button class="button-style"> GET IN TOUCH </button>
	<!-- <div class="img" /> -->
	<!-- <div class="text-area">
		<span class="h1"> ML something </span>
		<span class="h2">[CTA] Contact sales form</span>
		<span class="h3"
			>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
			labore et dolore magna aliqua. Ut
		</span>
		<div class="form">
			<input type="text" class="input" />
			<button class="button"> CTA</button>
		</div>
	</div> -->
</div>

<style>
	.work {
		font-weight: 500;
		font-size: 28px;
		line-height: 38px;
		padding-right: 110px;
		
		color: #000000;
	}
	.contact-container {
		border-radius: 20px;
		display: flex;
		/* width: 1120px; */
		height: 210px;
		background: #f7f9fc;
		margin-bottom: 155px;
		justify-content: center;
		/* padding-left: 138.5px; */
    align-items: center;
	}
	.input{
		width: 251px;
		height: 40px;
		border-radius: 8px;
		background: none;
		border-color: #787d8e;
		margin-right: 10px;
		border: 2px solid black;
		padding-left: 10px;
		color: #B3B3B3;
	}
	.button-style {
		border: none;
		width: 161px;
		font-weight: 500;
		font-size: 14px;
		height: 40px;
		color: #f7f9fc;

		/* Black & White/Pure black */

		background: #000000;
		border-radius: 8px;
	}

	.button-style:hover {
		background: #31343f;
	}
	.button-style:focus {
		background: #787d8e;
	}
	@media (max-width: 767px) {
		.contact-container {
			flex-direction: column;
			align-items: center;
			margin-left: 0;
		}
		.text-area {
			align-items: center;
			margin-left: 0;
		}
	}
</style>
