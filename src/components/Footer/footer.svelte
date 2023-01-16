<!-- Site footer -->
<footer class="footer-container">
	<div class="container">
		<div class="row">
			<div class="flex-20">
				<img src="images/brandLogoFooter.svg" alt="brandLogoFooter" />
			</div>

			<div class="flex-20">
				<h6 style="margin-bottom:20px">Products:</h6>
				<ul class="footer-links">
					<li><a href="#/">UniStore</a></li>
					<li><a href="#/">UniSearch</a></li>
					<li><a href="#/">UniForm</a></li>
				</ul>
			</div>

			<div class="flex-20">
				<h6 style="margin-bottom:20px">Technologies</h6>
				<ul class="footer-links">
					<li><a href="#/">UKV</a></li>
					<li><a href="#/">UJRPC</a></li>
					<li><a href="#/">UCSB</a></li>
				</ul>
			</div>
			<div class="flex-20">
				<h6 style="margin-bottom:20px">{null}</h6>
				<ul class="footer-links">
					<li><a href="#/">UCSB</a></li>
					<li><a href="#/">ADSB</a></li>
					<li><a href="#/">UCSet</a></li>
					<li><a href="#/">UModel</a></li>
				</ul>
			</div>
			<div class="flex-20">
				<h6 style="margin-bottom:20px">Resources</h6>
				<ul class="footer-links">
					<li><a href="#/">About</a></li>
					<li><a href="#/">Blog</a></li>
					<li><a href="#/">Careers</a></li>
					<li><a href="#/">Contact</a></li>
				</ul>
			</div>
		</div>
	</div>
	<div class="container">
		<hr style="border: 1px solid #CCCCCC;" />
		<div class="row">
			<div class="col-md-8 col-sm-6 col-xs-12" style="color:#B3B3B3">
				<p class="copyright-text">
					2015 - 2023 <span style="padding-left:32px">Terms of Use</span>
					<span style="padding-left:32px">Privacy Notice</span>
				</p>
			</div>

			<div class="col-md-4 col-sm-6 col-xs-12">
				<ul class="social-icons">
					<li><a href="#/"><img src="images/footerGit.svg" alt="github" /></a></li>
					<li><a href="#/"><img src="images/footerLinkedIn.svg" alt="linkedIn" /></a></li>
					<li><a href="#/"><img src="images/footerTwitter.svg" alt="twitter" /></a></li>
					<li><a href="#/"><img src="images/footerYoutube.svg" alt="youtube" /></a></li>
					<li><a href="#/"><img src="images/footerEmail.svg" alt="email" /></a></li>
				</ul>
			</div>
		</div>
	</div>
</footer>

<style>
	.footer-container {
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 80px 0px 32px;
		gap: 80px;
		height: 425px;
		background: #f7f9fc;
	}

	.flex-20 {
		width: 20%;
	}
	.footer-links {
		padding-left: 0;
		list-style: none;
	}
	.footer-links li {
		font-weight: 500;
		font-size: 16px;
		line-height: 24px;
		margin-bottom: 16px;

		color: #787d8e;
	}
	.footer-links a {
		text-decoration: none;
		color: #787d8e;
	}
	.footer-links a:active,
	.footer-links a:focus,
	.footer-links a:hover {
		color: black;
		text-decoration: none;
	}

	.site-footer .social-icons a {
		width: 40px;
		height: 40px;
		line-height: 40px;
		margin-left: 6px;
		margin-right: 0;
		border-radius: 100%;
		background-color: #33353d;
	}
	.copyright-text {
		margin: 0;
	}
	@media (max-width: 991px) {
	}
	@media (max-width: 767px) {
	}
	.social-icons {
		padding-left: 0;
		margin-bottom: 0;
		list-style: none;
	}
	.social-icons li {
		display: inline-block;
		margin-bottom: 4px;
	}

	.social-icons a {
		/* background-color:#eceeef; */
		color: #818a91;
		font-size: 16px;
		display: inline-block;
		line-height: 44px;
		width: 44px;
		height: 44px;
		text-align: end;
		margin-right: 8px;
		border-radius: 100%;
		-webkit-transition: all 0.2s linear;
		-o-transition: all 0.2s linear;
		transition: all 0.2s linear;
	}
	/* .social-icons a:active,.social-icons a:focus,.social-icons a:hover
{
  color:#fff;
  background-color:#29aafe
} */

	@media (max-width: 767px) {
	}
</style>
