<script lang="ts">
	export let h1;
	export let h2;
	export let h3;
	export let img;
	export let imgAlignLeft;
	export let features;
	export let Links;
</script>

<div class="container" style={`flex-direction:${imgAlignLeft === true ? 'row-reverse' : 'row'}`}>
	<div class="text-area">
		<div
			style="width: 32px;
        height: 32px;
        
        background: #D9D9D9;"
		/>
		<span class="h1"> {h1}</span>
		<span class="h2">{h2}</span>
		<span class="h3"> {h3}</span>

		<div class="features">
			{#each features as feature}
				<span
					style="width: 60px;
                    text-align: center;
      height: 22px;


      background: #F7F9FC;">{feature}</span
				>
			{/each}
		</div>

		<div class="links">
			{#each Links as Link}
				<span
					style="
                margin-right:20px;
font-size: 16px;
line-height: 24px;
color: #787D8E;
  ">{Link}</span
				>
			{/each}
		</div>
	</div>
	<img src={img} alt="" />
</div>

<style>
	.container {
		display: flex;
		margin-bottom: 200px;
	}
	.features {
		display: flex;
		/* justify-content: space-around; */
		font-size: 12px;
		line-height: 18px;
		margin-bottom: 34px;
		color: #787d8e;
	}
	.links {
		display: flex;
	}
	.text-area {
		display: flex;
		flex-direction: column;
		width: 453px;
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
		margin-bottom: 34px;
	}
</style>
