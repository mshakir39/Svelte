<script lang="js">
	import { Collapse, Navbar, NavbarToggler, NavbarBrand, Nav, NavItem, NavLink } from 'sveltestrap';

	let isOpen = false;

	// @ts-ignore
	function handleUpdate(event) {
		isOpen = event.detail.isOpen;
	}
</script>

<svelte:head>
	<link
		rel="stylesheet"
		href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css"
	/>
</svelte:head>

<Navbar color="dark" light expand="md" style="width: -webkit-fill-available;">
	<div style="display: flex;    width: -webkit-fill-available;">
		<NavbarBrand href="/" style="width:26%"
		><img
			src="/images/brandLogo.svg"
			alt="Unum"
			style="margin-left:60px;margin-right:175px;"
		/></NavbarBrand
	>
	<div class="flex-70">
		<NavbarToggler on:click={() => (isOpen = !isOpen)} style="position: sticky;
			left: 98%;" />

			<Collapse {isOpen} navbar expand="md" on:update={handleUpdate}>
				<Nav class="" navbar style="color:#fffff;display:flex;width: -webkit-fill-available;">
					<div class="flex-74">

						<NavItem style="">
							<span>
								<NavLink href="#/">Products</NavLink>
							</span>
						</NavItem>
						<NavItem>
							<span>
								<NavLink href="#">Technologies</NavLink>
							</span>
						</NavItem>
						<NavItem>
							<span>
								<NavLink href="#">Resources</NavLink>
							</span>
						</NavItem>
						<NavItem style="">
							<span>
								<NavLink href="#">Blog</NavLink>
							</span>
						</NavItem>
					</div>
				<div class="flex-26">
					<NavItem >
						<span>
							<NavLink href="#">GITHUB</NavLink>
						</span>
					</NavItem>
					<NavItem style="">
						<span>
							<NavLink href="#" style="color:white;white-space:nowrap">CONTACT SALES</NavLink>
						</span>
					</NavItem>
				</div>
					
				</Nav>
			</Collapse>

	</div>
	
	</div>
	
</Navbar>

<style>
	.flex-74{
width:74%;display:flex;justify-content:flex-start	
	}
	.flex-70{
		width:70%
	}
	.flex-26{
		width:26%;display:flex
	}
	@media (max-width: 767px) {
		:global(body) {
			width: max-content;
		}
	}
	@media (max-width: 1240px) {
		:global(body) {
			width: max-content;
		}
	}
	/* @media (max-width: 1366px) {
		:global(body) {
			width: max-content;
		}
	} */
	
	:global(body) {
			overflow-x: hidden;
		}
	span :global(a) {
		color: #787d8e;
		font-size: 16px;
	}

	span :global(a):hover {
		color: white;
	}
	@media (max-width: 767px) {
		.flex-74{
flex-direction: column;	
	}
	.flex-26{
		flex-direction: column;	

	}
	.flex-70{

	}
	}
</style>
