<script>
	let ClickedNavLinks = '';
	let ClickedHamMenu = '';

	function clickedNavbar() {
		ClickedNavLinks = ClickedNavLinks === '' ? 'clicked' : ''; //ternary operator to fill the variable content
		ClickedHamMenu = ClickedHamMenu === '' ? 'clicked' : ''; //if the statement is true, then ClickedHamMenu === "clicked"
	}
</script>

<div class="main-navbar">
	<a class="logos" href="/">
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
	</a>
	<!-- svelte-ignore a11y-click-events-have-key-events -->
	<div class="ham-menu {ClickedHamMenu}" on:click={clickedNavbar}>
		<span />
		<span />
		<span />
	</div>
	<ul class="nav-links {ClickedNavLinks}">
		<li><a href="/">Home</a></li>
		<li><a href="/history-section">History</a></li>
		<li><a href="/circuits-section">Circuits</a></li>
		<li><a href="/drivers-section">Drivers</a></li>
		<li><a href="/about-section">About</a></li>
	</ul>
</div>

<style>
	.main-navbar {
		width: 100%;
		height: 4rem;
		background-color: hsl(5, 100%, 50%);
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
		padding: 1rem 4rem;
		position: fixed;
	}
	a {
		color: white;
		transition: all 350ms ease-in-out;
	}

	.logos {
		display: flex;
		align-items: center;
		gap: 0.75rem;
	}
	.fia-logo {
		height: 2rem;
		filter: brightness(0) invert(1); /*inverting black colored images to white colored ones*/
	}
	.f1-logo {
		aspect-ratio: 4/1;
		height: 1.6rem;
	}
	.logos span {
		width: 2px;
		height: 1.4rem;
		background-color: hsl(0, 0%, 100%, 0.8);
		border-radius: 50rem;
	}

	.nav-links {
		display: flex;
		flex-direction: row;
		list-style-type: none;
		font-weight: 500;
		gap: 0.5rem;
	}
	.nav-links li {
		padding: 1rem;
		border-radius: 0.25rem;
		transition: all 350ms ease-in-out;
	}
	.nav-links li:hover {
		background-color: hsl(5, 100%, 36%);
	}
	.nav-links li:active {
		font-weight: 600;
	}
	.ham-menu {
		display: none;
	}

	@media screen and (max-width: 768px) {
		.main-navbar {
			padding: 1rem 2rem;
			z-index: 10;
		}

		.ham-menu {
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			gap: 0.325rem;
			z-index: 50;
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
			transform: rotate(45deg) translateY(8px);
		}
		.ham-menu.clicked span:nth-child(2) {
			transform: translateX(-35px);
			background: transparent;
		}
		.ham-menu.clicked span:nth-child(3) {
			transform: rotate(-45deg) translateY(-8.1px);
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
			padding: 5vh 5vw 20vh;
			height: 100vh;
			width: 40vw;
			/* decoration styles */
			background-color: hsl(5, 100%, 50%, 0.5);
			backdrop-filter: blur(2px);
			/* transition styles */
			transition: all 350ms ease-in-out;
			transform: translateX(100%);
		}
		.nav-links.clicked {
			transform: translateX(0);
            opacity: 1;
		}
	}
</style>
