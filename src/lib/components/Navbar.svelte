<script>
	import Icon from 'svelte-awesome';
	import arrowRight from 'svelte-awesome/icons/arrowRight';

	let ClickedNavLinks = '';
	let ClickedHamMenu = '';

	function clickedNavbar() {
		ClickedNavLinks = ClickedNavLinks === '' ? 'clicked' : ''; //ternary operator to fill the variable content
		ClickedHamMenu = ClickedHamMenu === '' ? 'clicked' : ''; //if the statement is true, then ClickedHamMenu === "clicked"
	}
</script>

<div class="main-navbar">
	<a class="logos" href="/" title="Home page">
		<div class="logos-container">
			<img
				class="fia-logo"
				src="https://www.formula1.com/etc/designs/fom-website/images/fia_logo.png"
				alt="Fédération Internationale de l'Automobile Logo"
			/>
			<span />
			<svg class="f1-logo" viewBox="0 0 320 80" xmlns="http://www.w3.org/2000/svg">
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M45.2583 80L80.7417 45.575H80.7333C94.7167 32.0167 100.392 29.9583 127.058 29.9583H233.408L264.008 0H123.025C87.3333 0 77.2417 3.4 56.3083 24.1167L0 80H45.2583ZM127.7 34.7417H228.842L200.792 62.7917H128.225C114.925 62.7917 111.983 63.4167 105.383 70.0167L95.4 80H53.4333L84.4583 48.975C96.6417 36.8 100.842 34.7417 127.7 34.7417ZM320 0L239.783 80H190.175L270.175 0H320ZM267.183 77.4667C268.85 79.1583 270.95 80 273.475 80C276 80 278.075 79.1583 279.717 77.4833C281.358 75.8083 282.175 73.7333 282.175 71.2667C282.175 68.8 281.35 66.725 279.7 65.0333C278.05 63.3417 275.967 62.5 273.442 62.5C270.917 62.5 268.825 63.3417 267.167 65.0167C265.508 66.6917 264.675 68.7667 264.675 71.2333C264.675 73.7 265.508 75.775 267.183 77.4667ZM268.225 66.025C269.625 64.5917 271.358 63.875 273.425 63.875C275.5 63.875 277.233 64.5917 278.625 66.025C280.017 67.4583 280.717 69.2 280.717 71.25C280.717 73.3 280.017 75.0333 278.625 76.4583C277.225 77.8833 275.5 78.5917 273.425 78.5917C271.35 78.5917 269.617 77.875 268.225 76.4417C266.833 75.0083 266.133 73.275 266.133 71.2333C266.133 69.1917 266.833 67.4583 268.225 66.025ZM271.717 76.125V72.6917L271.725 72.7H273.683L275.342 76.1333H277.367L275.542 72.45C276.158 72.1667 276.592 71.8 276.85 71.3417C277.108 70.8833 277.233 70.1833 277.233 69.2417C277.233 68.3 276.917 67.5917 276.283 67.125C275.65 66.65 274.7 66.4167 273.442 66.4167H269.792V76.125H271.717ZM271.683 71.1833V67.9167H273.275C274.65 67.9167 275.333 68.4583 275.333 69.55C275.333 70.125 275.2 70.5417 274.933 70.8C274.675 71.0583 274.242 71.1833 273.642 71.1833H271.683Z"
					fill="currentcolor"
				/>
			</svg>
		</div>
		<div class="arrow-menu">
			<Icon data={arrowRight} style="color: hsl(240, 67%, 2%);" />
		</div>
	</a>
	<!-- svelte-ignore a11y-click-events-have-key-events -->
	<div class="secondary-menu">
		<div class="ham-menu {ClickedHamMenu}" on:click={clickedNavbar}>
			<span />
			<span />
			<span />
		</div>
		<ul class="nav-links {ClickedNavLinks}">
			<li>
				<a href="/history">
					<p>History</p>
					<div class="arrow-menu-links">
						<Icon data={arrowRight} style="color: #f9f4f4;" />
					</div>
				</a>
			</li>
			<li>
				<a href="/circuits">
					<p>Circuits</p>
					<div class="arrow-menu-links">
						<Icon data={arrowRight} style="color: #f9f4f4;" />
					</div>
				</a>
			</li>
			<li>
				<a href="/drivers">
					<p>Drivers</p>
					<div class="arrow-menu-links">
						<Icon data={arrowRight} style="color: #f9f4f4;" />
					</div>
				</a>
			</li>
			<li>
				<a href="/about">
					<p>About</p>
					<div class="arrow-menu-links">
						<Icon data={arrowRight} style="color: #f9f4f4;" />
					</div>
				</a>
			</li>
		</ul>
	</div>
</div>

<style>
	.main-navbar {
		z-index: 999;
		width: 100%;
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 0.4rem;
		/* justify-content: space-between; */
		position: fixed;
		padding: 0.4rem;
	}
	a {
		color: white;
		transition: all 350ms ease-in-out;
	}

	.logos {
		/* layouting styles */
		display: flex;
		flex: 1;
		align-items: center;
		justify-content: space-between;
		gap: 0.75rem;
		height: 3.5rem;
		padding: 0.25rem;
		/* decorating styles */
		border-radius: 50rem;
		background-color: hsl(5, 100%, 50%);
		border: solid 3px hsl(0, 0%, 100%);
		outline: solid 1.5px hsl(240, 67%, 2%);
	}
	.logos-container {
		display: flex;
		flex-direction: row;
		align-items: center;
		padding: 0 0 0 1.25rem;
		gap: 1rem;
	}
	.fia-logo {
		height: 1.6rem;
		filter: brightness(0) invert(1); /*inverting black colored images to white colored ones*/
	}
	.f1-logo {
		aspect-ratio: 4/1;
		height: 1.5rem;
	}
	.logos-container span {
		width: 2px;
		height: 1.6rem;
		background-color: hsla(0, 0%, 93%, 0.8);
	}
	.arrow-menu {
		width: 5rem;
		height: 100%;
		background-color: hsla(0, 0%, 95%);
		border-radius: 50rem;
		display: grid;
		place-items: center;
	}

	.secondary-menu {
		display: flex;
		align-items: center;
		justify-content: flex-end;
		flex: 3;
		height: 3.5rem;
		border-radius: 50rem;
		padding: 0.2rem 0.3rem;
		border: solid 3px hsl(0, 0%, 100%);
		outline: solid 1.5px hsl(240, 67%, 2%);
		background-color: hsla(0, 0%, 95%);
	}

	.nav-links {
		display: flex;
		list-style-type: none;
		gap: 0.5rem;
	}

	.nav-links li a {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 1.25rem;
		padding: 0 0 0 1rem;
		color: hsl(240, 67%, 2%);
		font-weight: 500;
		height: 2.5rem;
		background-color: hsla(0, 0%, 95%);
		border-radius: 50rem;
		border: solid 3px hsl(0, 0%, 100%);
		outline: solid 1.5px hsl(240, 67%, 2%);
	}

	.arrow-menu-links  {
		width: 4rem;
		height: 100%;
		border-radius: 50rem;
		display: grid;
		place-items: center;
		transition: all 350ms ease-in-out;
	}

	.nav-links li:nth-child(1) a div {
		background-color: hsl(180, 97%, 23%);
	}
	.nav-links li:nth-child(2) a div {
		background-color: hsl(173, 100%, 17%);
	}
	.nav-links li:nth-child(3) a div {
		background-color: hsl(225, 54%, 23%);
	}
	.nav-links li:nth-child(4) a div {
		background-color: hsl(215, 89%, 14%);
	}

	.nav-links li:nth-child(1) a:hover div {
		background-color: hsl(180, 97%, 23%, 0.7);
	}
	.nav-links li:nth-child(2) a:hover div {
		background-color: hsl(173, 100%, 17%, 0.7);
	}
	.nav-links li:nth-child(3) a:hover div {
		background-color: hsl(225, 54%, 23%, 0.7);
	}
	.nav-links li:nth-child(4) a:hover div {
		background-color: hsl(215, 89%, 14%, 0.7);
	}

	.ham-menu {
		display: none;
	}

	@media screen and (max-width: 1024px) {
		.main-navbar {
			z-index: 10;
		}

		.logos {
			flex: 9;
		}
		.secondary-menu {
			flex: 1;
			justify-content: center;
			background-color: hsl(5, 100%, 50%);
		}

		.ham-menu {
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			gap: 0.325rem;
			z-index: 100;
		}
		.ham-menu span {
			width: 1.6rem;
			height: 0.175rem;
			border-radius: 50rem;
			background-color: white;
			transform-origin: center;
			transition: all 350ms ease-in-out;
		}
		.ham-menu.clicked span:nth-child(1) {
			transform: rotate(45deg) translateY(3.75px) translatex(5px);
		}
		.ham-menu.clicked span:nth-child(2) {
			transform: translateX(-35px);
			background: transparent;
		}
		.ham-menu.clicked span:nth-child(3) {
			transform: rotate(-45deg) translateY(-3.75px) translatex(5px);
		}

		.nav-links {
			/* positioning styles */
			position: absolute;
			z-index: 25;
			right: 0;
			top: 0;
			/* layouting styles */
			display: flex;
			flex-direction: column;
			align-items: right;
			justify-content: center;
			/* sizing styles */
			margin: 0.25rem 0 0.25rem 0;
			padding: 5vh 5vw 20vh;
			height: 100vh;
			width: 45vw;
			/* decoration styles */
			border-radius: 4rem 0 0 4rem;
			border: solid 3px hsl(0, 0%, 100%);
			outline: solid 1.5px hsl(240, 67%, 2%);
			background-color: hsla(0, 0%, 100%, 0.5);
			backdrop-filter: blur(4px);
			/* transition styles */
			transition: all 350ms ease-in-out;
			transform: translateX(101%);
		}

		.nav-links li a {
			gap: 0rem;
			width: 100%;
			justify-content: space-between;
		}

		.nav-links.clicked {
			transform: translateX(0);
			opacity: 1;
		}
	}
</style>
