<script>
	import Card, { Content, PrimaryAction, Actions, ActionButtons } from '@smui/card';
	import Chip, { Text } from '@smui/chips';

	export let details = {
		title: '',
		description: '',
		status: '',
		lang: '',
		stars: 0,
		shares: 0
	};
	const { title, description, status, lang, stars, shares } = details;

	let clicked = 0;
</script>

<div class="card-display">
	<div class="card-container">
		<Card style="background: #F7F9FC;box-shadow:none">
			<PrimaryAction on:click={() => clicked++}>
				<Content class="mdc-typography--body2">
					<img src="/images/github.png" alt="Github" style="margin-bottom:12px"/>
					<h2 class="mdc-typography--headline6 card-title">
					<img src="images/book.svg" alt="book" style="margin-right:9.81px"/>	{title}
						<!-- <Chip
							chip={status}
							style="border-radius: unset;
						text-transform: capitalize;
						font-size: 12px;
						margin-left: 10px;
						height: 25px;"
						>
							<Text>{status}</Text>
						</Chip> -->
					</h2>
					<div class="card-description">
						{description}
					</div>
				</Content>
			</PrimaryAction>
			<Actions>
				<ActionButtons>
					<Chip
						chip={lang}
						style="    background: unset;
					display: flex;
					justify-content: space-between;
					min-width: 70px;"
					>
						<img src="/images/rectangle.png" alt="rectangle" />
						<Text tabindex={0}>{lang}</Text>
					</Chip>
					<Chip
						chip={stars}
						style="    background: unset;
					display: flex;
					justify-content: space-between;
					min-width: 65px;"
					>
						<img src="/images/star.png" alt="rectangle" />
						<Text tabindex={0}>{stars}</Text>
					</Chip>
					<Chip
						chip={lang}
						style="    background: unset;
					display: flex;
					justify-content: space-between;
					min-width: 60px;"
					>
						<img src="/images/share.png" alt="rectangle" />
						<Text tabindex={0}>{shares}</Text>
					</Chip>
				</ActionButtons>
			</Actions>
		</Card>
	</div>
</div>

<style>
	.card-display {
		width: 400px;
		margin-bottom: 40px;
	}
	.card-title {
		margin: 0;
		display: flex;
		font-size: 18px;
	}
	.card-description {
		padding-top: 10px;
		color: #787d8e;
		font-size: 14px;
	}
</style>
