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
	<NavbarBrand href="/"
		><img
			src="/images/brandLogo.svg"
			alt="Unum"
			style="margin-left:60px;margin-right:175px;"
		/></NavbarBrand
	>
	<NavbarToggler on:click={() => (isOpen = !isOpen)} />
	<Collapse {isOpen} navbar expand="md" on:update={handleUpdate}>
		<Nav class="ms-auto" navbar style="color:#fffff">
			<NavItem>
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
			<NavItem style="margin-right:428px">
				<span>
					<NavLink href="#">Blog</NavLink>
				</span>
			</NavItem>
			<NavItem>
				<span>
					<NavLink href="#">GITHUB</NavLink>
				</span>
			</NavItem>
			<NavItem>
				<span>
					<NavLink href="#" style="color:white;white-space:nowrap">CONTACT SALES</NavLink>
				</span>
			</NavItem>
		</Nav>
	</Collapse>
</Navbar>

<style>
	@media (max-width: 767px) {
		:global(body) {
			width: max-content;
		}
	}

	span :global(a) {
		color: #787d8e;
		font-size: 16px;
	}

	span :global(a):hover {
		color: white;
	}
</style>
