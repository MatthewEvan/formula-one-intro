<script lang="ts">
	import MercedesW14 from '$assets/main-page/Mercedes-W14.png';
	import RedBullRB19 from '$assets/main-page/RedBull-RB19.png';
	import GridLinesDeco from '$assets/main-page/Gridlines Deco.png';

	import Icon from 'svelte-awesome';
	import angleDown from 'svelte-awesome/icons/angleDown';
	import angleDoubleRight from 'svelte-awesome/icons/angleDoubleRight';
	import externalLink from 'svelte-awesome/icons/externalLink';
</script>

<div class="main-page">
	<section id="header">
		<div class="circle-bg">
			<span />
			<span />
			<span />
		</div>
		<div class="main-header">
			<img src={MercedesW14} alt="Mercedes AMG Petronas F1 W14" class="mercedesw14" />
			<div class="header-text">
				<a href="https://www.formula1.com/" target="_blank" title="Formula One Website">
					<svg
						class="f1-logo"
						width="10rem"
						viewBox="0 0 320 80"
						xmlns="http://www.w3.org/2000/svg"
					>
						<path
							fill-rule="evenodd"
							clip-rule="evenodd"
							d="M45.2583 80L80.7417 45.575H80.7333C94.7167 32.0167 100.392 29.9583 127.058 29.9583H233.408L264.008 0H123.025C87.3333 0 77.2417 3.4 56.3083 24.1167L0 80H45.2583ZM127.7 34.7417H228.842L200.792 62.7917H128.225C114.925 62.7917 111.983 63.4167 105.383 70.0167L95.4 80H53.4333L84.4583 48.975C96.6417 36.8 100.842 34.7417 127.7 34.7417ZM320 0L239.783 80H190.175L270.175 0H320ZM267.183 77.4667C268.85 79.1583 270.95 80 273.475 80C276 80 278.075 79.1583 279.717 77.4833C281.358 75.8083 282.175 73.7333 282.175 71.2667C282.175 68.8 281.35 66.725 279.7 65.0333C278.05 63.3417 275.967 62.5 273.442 62.5C270.917 62.5 268.825 63.3417 267.167 65.0167C265.508 66.6917 264.675 68.7667 264.675 71.2333C264.675 73.7 265.508 75.775 267.183 77.4667ZM268.225 66.025C269.625 64.5917 271.358 63.875 273.425 63.875C275.5 63.875 277.233 64.5917 278.625 66.025C280.017 67.4583 280.717 69.2 280.717 71.25C280.717 73.3 280.017 75.0333 278.625 76.4583C277.225 77.8833 275.5 78.5917 273.425 78.5917C271.35 78.5917 269.617 77.875 268.225 76.4417C266.833 75.0083 266.133 73.275 266.133 71.2333C266.133 69.1917 266.833 67.4583 268.225 66.025ZM271.717 76.125V72.6917L271.725 72.7H273.683L275.342 76.1333H277.367L275.542 72.45C276.158 72.1667 276.592 71.8 276.85 71.3417C277.108 70.8833 277.233 70.1833 277.233 69.2417C277.233 68.3 276.917 67.5917 276.283 67.125C275.65 66.65 274.7 66.4167 273.442 66.4167H269.792V76.125H271.717ZM271.683 71.1833V67.9167H273.275C274.65 67.9167 275.333 68.4583 275.333 69.55C275.333 70.125 275.2 70.5417 274.933 70.8C274.675 71.0583 274.242 71.1833 273.642 71.1833H271.683Z"
							fill="#FF1801"
						/>
					</svg>
				</a>
				<h1><span>Formula One</span></h1>
				<h2>
					The <span>pinnacle</span> of
					<span>motorsport</span> where every race requires
					<span>talent</span>
					and <span>technophiles.</span>
				</h2>
				<div class="header-desc">
					<div class="img-grid">
						<img
							src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c2/Johnny_Herbert_1995_Britain.jpg/330px-Johnny_Herbert_1995_Britain.jpg"
							alt="Silverstone Circuit 1"
						>
						<img
							src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/McLaren_MP4_at_Silverstone_Classic_2011.jpg/330px-McLaren_MP4_at_Silverstone_Classic_2011.jpg"
							alt="Silverstone Circuit 2"
						>
						<img
							src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b0/Keke_Rosberg_Williams_FW10_1985_German_GP.jpg/330px-Keke_Rosberg_Williams_FW10_1985_German_GP.jpg"
							alt="Silverstone Circuit 3"
						>
					</div>
					<p>
						Firstly held at the Silverstone Circuit on 13th of May 1950, Formula One has since been
						one of the most prestigious and innovative motorsport championship league with almost
						171 teams and 774 drivers on 60+ different circuits around the world
					</p>
				</div>
				<div class="discover-more">
					<a href="#content-overview">Discover More<Icon data={angleDown} scale={1.25} style="color: hsl(0, 0%, 95%)"/></a>
				</div>
			</div>
			<img src={RedBullRB19} alt="Red Bull RB19" class="redbullrb19" />
		</div>
	</section>
	<section id="content-overview">
		<div class="part-01">
			<div class="title-01">
				<h2>01</h2>
				<p>How It <br />Works<br /></p>
			</div>
			<p class="description-01">
				All events and preparations needed to be done by every teams in a usual F1 race weekend,
				consisting of Free Practice, Qualifying, and the Main Race.
			</p>
			<a href="#howitworks">
				<Icon data={angleDoubleRight} scale={2} />
			</a>
			<img
				src="https://www.pngmart.com/files/22/F1-Ferrari-Transparent-PNG.png"
				alt="Ferrari F1 Car"
			/>
		</div>
		<div class="other-sections">
			<div class="tile-column-1">
				<a class="part-02 heading-text-link" href="/circuits">
					<div>
						<h2>02</h2>
						<Icon data={angleDoubleRight} scale={2} />
					</div>
					<p>Circuits</p>
				</a>
				<a class="part-03 heading-text-link" href="/teams">
					<div>
						<h2>03</h2>
						<Icon data={angleDoubleRight} scale={2} />
					</div>
					<p>Teams</p>
				</a>
			</div>
			<div class="tile-column-2">
				<a class="part-04 heading-text-link" href="/drivers">
					<div>
						<h2>04</h2>
						<Icon data={angleDoubleRight} scale={2} />
					</div>
					<p>Drivers</p>
				</a>
				<a class="part-05 heading-text-link" href="/about">
					<div>
						<h2>05</h2>
						<Icon data={angleDoubleRight} scale={2} />
					</div>
					<p>About</p>
				</a>
			</div>
		</div>
	</section>
	<section id="racing-stripes">
		<div class="racing-stripes-deco"></div>
		<div class="racing-stripes-deco"></div>
		<div class="racing-stripes-deco"></div>
		<div class="racing-stripes-deco"></div>
		<div class="racing-stripes-deco"></div>
	</section>
	<section id="howitworks">
		<h3>How It Works</h3>
		<div class="event-overview">
			<div class="event-tiles">
				<div class="event-header">
					<h4>Free Practice</h4>
					<img src={GridLinesDeco} alt="Gridlines Decoration">
					<p>Every team gets a chance to test their cars on the specific circuit to adjust its settings according to the weather condition there</p>
				</div>
				<img src="https://d3cm515ijfiu6w.cloudfront.net/wp-content/uploads/2022/04/04101702/lewis-hamilton-leaves-garage-planetf1.jpg" alt="Free Practice Session of Mercedes AMG F1">
			</div>
			<div class="event-tiles">
				<div class="event-header">
					<h4>Qualifying</h4>
					<img src={GridLinesDeco} alt="Gridlines Decoration">
					<p>The event where every drivers attempted to score the fastest lap time with to determine their starting position the next day</p>
				</div>
				<img src="https://d3cm515ijfiu6w.cloudfront.net/wp-content/uploads/2023/03/09115251/red-bull-max-verstappen-2022-emilia-romagna-grand-prix-imola-planet-f1.jpg" alt="F1 Qualifying Session">
			</div>
			<div class="event-tiles">
				<div class="event-header">
					<h4>Grand Prix</h4>
					<img src={GridLinesDeco} alt="Gridlines Decoration">
					<p>The main event everyone’s waiting for, where every drivers battle and overtake others to be the first and win the race</p>
				</div>
				<img src="https://media.formula1.com/image/upload/f_auto/q_auto/v1682327140/interlagos-start-2022.png.transform/9col/image.png" alt="F1 Main Race - Grand Prix">
			</div>
		</div>
		<div class="event-description">
			<div class="event-desc-section free-practice">
				<div class="event-desc-text">
					<div class="event-desc-header">
						<h4>Free Practice</h4>
						<h5>/friː ˈpræktɪs/</h5>
					</div>
					<div class="event-desc-detail">
						<p>There are <b>three 60-minute free practice sessions</b> (two on Friday, one on Saturday) before an F1 Grand Prix where drivers and teams can run laps. 
						These sessions are crucial because <b>teams need to perfect their car setups</b>, gather data for the race, and test the true pace of the car for qualifying.</p>
						<div class="event-desc-conclusion">
							<p>So, on a usual race weekend, there will be :</p>
							<p>FRIDAYS : FP1 & FP2</p>
							<p>SATURDAYS : FP3</p>
						</div>
					</div>
				</div>
				<img src="https://www.goodwood.com/globalassets/.road--racing/race/modern/2022/6-june/f1-2023-calendar/monaco-gp-2023-mark-sutton-mi-30052023.jpg?crop=(0,0,2600,1463)&width=1600" alt="F1 Free Practice at Monaco">
			</div>
			<div class="event-desc-section qualifying">
				<div class="event-desc-text">
					<div class="event-desc-header">
						<h4>Qualifying</h4>
						<h5>/ˈkwɒlɪfaɪɪŋ/</h5>
					</div>
					<div class="event-desc-detail">
						<p>The whole qualifying session is used <b>to determine every driver’s starting position for the main race</b>, from the first position (P1) until the last position (P20). 
						F1 uses a knock-out qualifying system that’s <b>divided into three sessions ranging from 12 minutes - 18 minutes</b>, where some drivers are eliminated </p>
						<div class="event-desc-conclusion">
							<p>So, on a usual race weekend, there will be :</p>
							<ul>
								<li>&#8226 Q1: P20-P16</li>
								<li>&#8226 Q2: P15-P11</li>
								<li>&#8226 Q3: P10-P1</li>
							</ul>
						</div>
					</div>
				</div>
				<img src="https://d3cm515ijfiu6w.cloudfront.net/wp-content/uploads/2023/01/31162230/abu-dhabi-2022-grid-planetf1.jpg" alt="F1 Qualifying at one of its circuit">
			</div>
			<div class="event-desc-section grand-prix">
				<div class="event-desc-text">
					<div class="event-desc-header">
						<h4>Grand Prix</h4>
						<h5>/ɡrænd priː/</h5>
					</div>
					<div class="event-desc-detail">
						<div class="grand-prix-header">
							<p>The main race everyone’s waiting for, where <b>every driver overtakes their rivals to be the first in the race</b>. P1 - P10 finishers gets some championship points that’ll determine their overall position</p>
							<p>So, these are the points awarded to every driver based on their finised position:</p>
						</div>
						<div class="event-desc-conclusion">
							<ul>
								<li><span>#01</span>25 pts</li>
								<li><span>#02</span>18 pts</li>
								<li><span>#03</span>15 pts</li>
								<li><span>#04</span>12 pts</li>
								<li><span>#05</span>10 pts</li>
								<li><span>#06</span>8 pts</li>
								<li><span>#07</span>6 pts</li>
								<li><span>#08</span>4 pts</li>
								<li><span>#09</span>2 pts</li>
								<li><span>#10</span>1 pts</li>
							</ul>
						</div>
					</div>
				</div>
				<img src="https://foxtelgroup.com.au/assets/article/mainImage/_1200xAUTO_fit_center-center_none/4k-main.jpg" alt="F1 Qualifying at one of its circuit">
			</div>
		</div>
	</section>
</div>

<style>
	/* #header #header #header */
	.main-page {
		margin: 2rem 4rem;
		color: hsl(0, 0%, 95%);
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	a {
		color: hsl(0, 0%, 95%);
	}

	#header {
		margin: 2rem 0rem 4rem;
		position: relative;
		z-index: 5;
	}

	.circle-bg span {
		position: absolute;
		aspect-ratio: 1/1;
		filter: blur(100px);
		z-index: -999;
		border-radius: 100%;
	}
	.circle-bg span:nth-child(1) {
		width: 20vw;
		top: 10vh;
		right: 2vw;
		background-color: #308ad9;
		opacity: 0.75;
	}
	.circle-bg span:nth-child(2) {
		width: 15vw;
		top: 5vh;
		left: 2vw;
		background-color: #72f7e5;
		opacity: 0.75;
	}
	.circle-bg span:nth-child(3) {
		width: 40vw;
		top: 8vh;
		left: 20vw;
		background-color: #6c0c26;
		opacity: 0.75;
	}

	.main-header {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
		gap: 5rem;
	}
	.header-text {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1rem;
		line-height: 1;
	}
	.mercedesw14,
	.redbullrb19 {
		height: 75vh;
	}
	.header-text h1 {
		color: hsl(0, 0%, 95%);
		font-size: 3rem;
		text-align: center;
		font-weight: 700;
	}
	.header-text h1 span {
		font-size: 4.75rem;
		font-weight: 900;
		background-image: linear-gradient(-135deg, #ea1b00, #f91d00, #f21c00, #cb1700, #a91400);
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
	}
	.header-text h2 {
		font-size: 2rem;
		text-align: center;
		padding-bottom: 1.25rem;
		border-bottom: 2px solid #dadada;
		line-height: 1.05;
	}

	.header-text h2 span {
		font-size: 2rem;
		font-family: 'Space Grotesk', monospace;
		text-decoration-line: underline;
		text-decoration-thickness: 0.25rem;
	}
	.header-text h2 span:nth-child(1) {
		text-decoration-color: hsla(59, 100%, 62%, 0.5);
	}
	.header-text h2 span:nth-child(2) {
		text-decoration-color: hsla(0, 100%, 47%, 0.5);
	}
	.header-text h2 span:nth-child(3) {
		text-decoration-color: hsla(234, 98%, 53%, 0.5);
	}
	.header-text h2 span:nth-child(4) {
		text-decoration-color: hsla(128, 100%, 47%, 0.5);
	}

	.header-desc {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	.header-desc p {
		color: #dadada;
		line-height: 1.15;
		font-weight: 500;
		font-size: 1.1rem;
		text-align: center;
		margin-bottom: 1rem;
		font-family: 'Space Grotesk', monospace;
	}
	.header-desc .img-grid {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 0.75rem;
		margin-inline: 1rem;
		margin-top: 0.25rem;
	}
	.header-desc .img-grid img {
		flex: 1;
		display: block;
		width: 100%;
		height: 5rem;
		object-fit: cover;
		object-position: center;
		border-radius: 0.25rem;
	}

	.discover-more {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 2rem;
	}
	.discover-more a {
		font-size: 1.125rem;
		font-weight: 700;
		color: hsl(0, 0%, 100%);
		padding: 1rem 2rem;
		background-image: linear-gradient(-135deg, #ea1b00, #f91d00, #f21c00, #cb1700, #a91400);
		border-radius: 50rem;
		transition: all 350ms ease-in-out;
		display: flex;
		gap: 0.75rem;
		align-items: center;
	}
	.discover-more a:hover {
		background-image: linear-gradient(-90deg, #ea1b00, #f91d00, #f21c00, #cb1700, #a91400);
		box-shadow: 1px 1px 8px hsla(0, 0%, 6%, 0.75);
	}

	/* Table of Contents Section */
	#content-overview {
		display: flex;
		align-items: stretch;
		gap: 1.5rem;
		margin-bottom: 4rem;
	}

	#content-overview .part-01 {
		display: flex;
		flex-direction: column;
		align-items: start;
		gap: 1rem;
		flex: 1;
		background-color: #d96459;
		border-radius: 0.5rem;
		padding: 1rem 2rem 2rem;
		position: relative;
		overflow: hidden;
	}

	.part-01 img {
		position: absolute;
		opacity: 0.8;
		width: 50vw;
		bottom: -5rem;
		right: -15rem;
		transform: scaleX(-1);
	}
	.part-01 .title-01 {
		display: flex;
		align-items: center;
		gap: 2rem;
	}
	.part-01 .title-01 h2 {
		font-family: 'Space Grotesk', monospace;
		font-size: 8rem;
		font-weight: 700;
		line-height: 1;
	}
	.part-01 .title-01 p {
		font-family: 'Space Grotesk', monospace;
		font-size: 4rem;
		line-height: 0.9;
		font-weight: 700;
	}
	.description-01 {
		margin: 0 4rem 2rem 0;
	}
	.part-01 > a {
		padding: 1rem 2rem;
		display: grid;
		place-items: center;
		border-radius: 0.5rem;
		background-color: #d7483b;
	}

	.other-sections {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: stretch;
		gap: 1.5rem;
	}
	.tile-column-1,
	.tile-column-2 {
		display: flex;
		flex: 1;
		align-items: strecth;
		gap: 1.5rem;
	}
	.heading-text-link {
		flex: 1;
		border-radius: 0.5rem;
		padding: 1rem;
		transition: all 350ms ease-in-out;
		display: flex;
		flex-direction: column;
		justify-content: start;
		gap: 0.5rem;
	}
	.part-02 {
		background-color: #bf0a19;
	}
	.part-03 {
		background-color: #d90b0b;
	}
	.part-04 {
		background-color: #bf9663;
	}
	.part-05 {
		background-color: #191826;
	}
	.heading-text-link:hover {
		scale: 1.04;
	}
	.heading-text-link:not(:hover) {
		opacity: 0.9;
	}
	.heading-text-link div {
		display: flex;
		align-items: center;
		justify-content: space-between;
		margin-right: 2rem;
	}
	.heading-text-link div h2 {
		font-family: 'Space Grotesk', monospace;
		font-weight: 700;
		font-size: 6rem;
		line-height: 1;
	}
	.heading-text-link p {
		font-size: 1.5rem;
		margin-left: 0.5rem;
		font-family: 'Space Grotesk', monospace;
		font-weight: 700;
	}

	/* Racing Stripes Decorations  */
	#racing-stripes {
		width: 100%;
	}
	#racing-stripes .racing-stripes-deco {
		width: 100%;
		height: 1rem;
		background: repeating-linear-gradient(
  			to right,
 			hsl(0, 0%, 95%),
  			hsl(0, 0%, 95%) 40px,
  			hsl(240, 11%, 7%) 40px,
  			hsl(240, 11%, 7%) 80px
		);
	}
	#racing-stripes .racing-stripes-deco:nth-child(2),
	#racing-stripes .racing-stripes-deco:nth-child(4) {
		background: repeating-linear-gradient(
  			to right,
			hsl(240, 11%, 7%),
			hsl(240, 11%, 7%) 40px,
			hsl(0, 0%, 95%) 40px,
  			hsl(0, 0%, 95%) 80px
		);
	}


	/* How it works Intro Section  */
	#howitworks {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 2rem;
		margin-top: 4rem;
		margin-bottom: 2rem;
	}
	#howitworks > h3 {
		font-size: 3.5rem;
		font-weight: 800;
		text-align: center;
	}

	.event-overview {
		display: flex;
		align-items: stretch;
		gap: 1.5rem;
		padding-bottom: 3rem;
		border-bottom: 0.25rem solid hsl(0, 0%, 95%);
	}
	.event-tiles {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 2rem;
		padding: 2rem 1.5rem;
		background-color: hsl(0, 100%, 30%);
		border-radius: 0.25rem;
	}
	.event-tiles:nth-child(2) {
		background-color: hsl(0, 100%, 40%);
	}
	.event-tiles > img {
		width: 80%;
		height: 2/1; /* sementara */
		border-radius: 0.5rem;
		opacity: 0.9;
		transition: all 350ms ease-in-out;
		object-fit: cover;
	}
	.event-tiles > img:hover {
		scale: 1.025;
		opacity: 1;
	}

	.event-header {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 0.5rem;
	}
	.event-header h4 {
		font-size: 2.5rem;
		font-family: "Space Grotesk", monospace;
	}
	.event-header p {
		text-align: center;
		font-family: "Space Grotesk", monospace;
	}
	.event-header img {
		width: 85%;
		height: 3rem;
		object-fit: cover;
		margin-bottom: 1rem
	}

	/* EVENT DESCRIPTIONS LAST PART  */
	.event-description {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1rem;
	}

	.event-desc-section {
		display: flex;
		gap: 3rem;
		align-items: center;
		background-color: hsla(0, 100%, 30%, 0.5);
		border-radius: 0.5rem;
		padding: 1.5rem 3rem;
	}
	.event-desc-section img {
		flex: 1;
		width: 20vw;
		aspect-ratio: 2/1;
		border-radius: 0.25rem;
		object-fit: cover;
	}
	.qualifying {
		flex-direction: row-reverse;
		background-color: hsla(0, 100%, 40%, 0.75)
	}

	.event-desc-text {
		display: flex;
		flex-direction: column;
		align-items: start;
		gap: 1.5rem;
		flex: 2
	}
	.event-desc-header {
		display: flex;
		align-items: end;
		gap: 1rem;
	}
	.event-desc-header h4 {
		font-size: 3rem;
		line-height: 1;
	}
	.event-desc-header h5 {
		font-size: 1.75rem;
		font-weight: 600;
		color: #C2F86B;
	}

	.event-desc-detail {
		display: flex;
		align-items: start;
		gap: 1.5rem;
	}
	.event-desc-detail * {
		font-family: "Space Grotesk", monospace;
	}
	.event-desc-detail p {
		flex: 2;
	}
	.event-desc-conclusion {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: start;
		gap: 0.5rem;
	}

	.event-desc-conclusion p:nth-child(2),
	.event-desc-conclusion p:nth-child(3) {
		font-size: 1.25rem;
		font-weight: 700;
		line-height: 1;
	}
	.event-desc-conclusion p:nth-child(2) {
		color: #CDFBCC;
	}
	.event-desc-conclusion p:nth-child(3) {
		color: #FBE0CC;
	}

	/* QUALIFYING DESCRIPTIONS  */
	.qualifying .event-desc-conclusion ul {
		display: flex;
		flex-direction: column;
		gap: 0.2rem;
		list-style-type: none;
		font-weight: 700;
		line-height: 1;
	}
	.qualifying .event-desc-conclusion ul li {
		font-size: 1.25rem;
	}
	.qualifying .event-desc-conclusion ul li:nth-child(1) {
		color: #CDFBCC;
	}
	.qualifying .event-desc-conclusion ul li:nth-child(2) {
		color: #F7FBCC;
	}
	.qualifying .event-desc-conclusion ul li:nth-child(3) {
		color: #F7CCFB;
	}
	
	/* GRAND PRIX SECTION  */
	.grand-prix .event-desc-detail {
		align-items: center;
	}
	.grand-prix .event-desc-detail .grand-prix-header {
		flex: 1;
	}
	.grand-prix .event-desc-conclusion {
		flex: 1;
	}
	.grand-prix .event-desc-conclusion ul {
		list-style: none;
		columns: 2;
		column-gap: 1.25rem;
	}
	.grand-prix .event-desc-conclusion ul li {
		display: flex;
		align-items: center;
		gap: 0.35rem;
		font-size: 1.25rem;
		font-weight: 700;
		color: #CDFBCC;
	}
	.grand-prix .event-desc-conclusion ul li span {
		color: #4fff4c;
		padding-right: 0.5rem;
	}
	.grand-prix-header {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}

	@media screen and (max-width: 1024px) {
		.main-page {
			margin: 2rem;
		}

		.main-header {
			gap: 1.5rem;
		}

		.mercedesw14,
		.redbullrb19 {
			height: 60vh;
		}
		.header-text h1 {
			font-size: 2.5rem;
		}
		.header-text h1 span {
			font-size: 3.5rem;
		}

		#content-overview {
			flex-direction: column;
		}
		.part-01 img {
			width: 60vw;
			bottom: -4rem;
			right: -8rem;
		}

		#howitworks {
			margin-inline: 3rem;
		}
		.event-overview {
			flex-direction: column;
		}
		.event-tiles {
			flex-direction: row;
		}
		.event-header {
			flex: 1;
		}
		.event-tiles > img {
			flex: 1;
			display: block;
			width: 50vw;
			aspect-ratio: 5/2.5;
		}
		.event-tiles:nth-child(2) {
			flex-direction: row-reverse
		}

		.event-desc-text {
			flex: 1;
		}
		.event-desc-section img {
			flex: 1;
			width: 35vw;
			aspect-ratio: 1/1;
		}
		.event-desc-header {
			flex-direction: column;
			align-items: start;
		}
		.event-desc-detail {
			flex-direction: column;
		}
	}

	@media screen and (max-width: 768px) {
		#header {
			margin: 2rem 2.5rem 4rem;
		}

		.main-header {
			flex-direction: column;
			gap: 0;
		}
		.mercedesw14,
		.redbullrb19 {
			display: none;
		}
		.header-desc .img-grid {
			display: flex;
			flex-direction: column;
		}
		.header-desc .img-grid img {
			aspect-ratio: 3/1;
		}

		.heading-text-link div {
			margin-right: 0;
		}
		.heading-text-link div h2 {
			font-size: 3rem;
		}
		.heading-text-link p {
			font-size: 1.25rem;
		}
		.part-01 img {
			width: 70vw;
			bottom: -3rem;
			right: -4rem;
		}
		.part-01 .title-01 h2 {
			font-size: 6rem;
		}
		.part-01 .title-01 p {
			font-size: 2.5rem;
		}

		#howitworks {
			margin: 3rem 2rem 2rem 2rem;
		}
		.event-tiles {
			flex-direction: column;
		}
		.event-tiles:nth-child(2) {
			flex-direction: column;
		}
		.event-tiles > img {
			flex: 1;
			width: 65vw;
			aspect-ratio: 5/2.5;
		}

		.event-desc-section {
			flex-direction: column;
			padding: 1.5rem 1.5rem;
		}
		.qualifying {
			flex-direction: column;
		}
		.event-desc-section img {
			width: 75vw;
			aspect-ratio: 5/2;
		}
		.event-desc-header h4 {
			font-size: 2.5rem;
		}
		.event-desc-header h5 {
			font-size: 1.5rem;
		}
	}
</style>
