<script lang="ts">
	import MercedesW14 from '$assets/main-page/Mercedes-W14.png';
	import RedBullRB19 from '$assets/main-page/RedBull-RB19.png';

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
					<span>motorsport</span> where every
					race requires
					<span>talent</span>
					and <span>technophiles.</span>
				</h2>
				<div class="header-desc">
					<div class="img-grid">
						<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c2/Johnny_Herbert_1995_Britain.jpg/330px-Johnny_Herbert_1995_Britain.jpg" alt="Silverstone Circuit 1">
						<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/McLaren_MP4_at_Silverstone_Classic_2011.jpg/330px-McLaren_MP4_at_Silverstone_Classic_2011.jpg" alt="Silverstone Circuit 2">
						<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b0/Keke_Rosberg_Williams_FW10_1985_German_GP.jpg/330px-Keke_Rosberg_Williams_FW10_1985_German_GP.jpg" alt="Silverstone Circuit 3">
					</div>
					<p>
						Firstly held at the Silverstone Circuit on 13th of May 1950, Formula One has since been
						one of the most prestigious and innovative motorsport championship league with almost 171
						teams and 774 drivers on 60+ different circuits around the world
					</p>
				</div>
				<div class="discover-more">
					<a href="#content-overview">Discover More<Icon data={angleDown} scale={1.25} style="color: hsl(0, 0%, 95%)" /></a>
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
				All the rules and regulations that are implemented inside every Formula One races, so races
				are fair and enjoyable for all participating in it
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
	<section id="howitworks">
		<div class="how-intro">
			<div class="how-intro-desc">
				<h3>How It Works</h3>
				<p>
					A regular Formula One Race Weekend usually consists of 3 sessions that's divided into 3
					days of the weekend, which are Fridays, Saturdays, and Sundays with different excitement
					and races altogether
				</p>
				<ul class="days-of-races">
					<li>Race Weekend Activities</li>
					<li><span>1</span>Fridays :<span>FP1 & FP2</span></li>
					<li><span>2</span>Saturdays:<span>FP3 & Qualifying</span></li>
					<li><span>3</span>Fridays :<span>Main Race Day</span></li>
				</ul>
			</div>
			<img
				src="https://cdn.crash.net/styles/article/s3/pa/3243856.0064.jpg?itok=3MaaXpcU"
				alt="Racing Scenes"
			/>
		</div>
		<div class="practice-quali">
			<div class="free-practice fp-quali">
				<div class="main-title">
					<h4>Free Practice</h4>
					<p>/friː ˈpræktɪs/</p>
				</div>
				<p>
					Free Practice are sessions that are used by teams to freely test their car settings and
					capabilities around the track, to adjust the car to its best before the main race and
					qualifying starts which will benefit the teams
				</p>
				<div class="fp-sessions">
					<ul>
						<li><span>1</span>Free Practice 1</li>
						<li><span>2</span>Free Practice 2</li>
						<li><span>3</span>Free Practice 3</li>
					</ul>
					<img
						src="https://www.formula1.com/content/dam/fom-website/manual/Misc/2020/2020races/Austria/F1AUT20jm_101.jpg.transform/6col/image.jpg"
						alt="Free Practice Session"
					/>
				</div>
			</div>
			<div class="qualifying fp-quali">
				<div class="main-title">
					<h4>Qualifying</h4>
					<p>/ˈkwɒlɪfaɪɪŋ/</p>
				</div>
				<p>
					Qualifying is a session that is really important because this determines the position of
					each driver's car in the race before from the first until the twentieth position.
					Qualifying is also divided into three sessions
				</p>
				<div class="quali-sessions">
					<ul>
						<li><span>1</span>P20-P16 position determined</li>
						<li><span>2</span>P15-P11 position determined</li>
						<li><span>3</span>P10-P1 position determined</li>
					</ul>
					<img
						src="https://img.sportstars.id//2021/07/WK781L/master_7nzC7bz437_1701.JPG"
						alt="Qualifying Session"
					/>
				</div>
			</div>
		</div>
		<div class="main-race">
			<div class="layout-race">
				<div class="main-race-desc">
					<div class="main-title">
						<h4>Main Race</h4>
						<p>/meɪn reɪs/</p>
					</div>
					<p>
						The day all Formula One fans are waiting for, which is the race day where all cars race
						for almost 1+ hours of 50+ laps around a circuit to get the <b>First Place</b>
					</p>
					<div class="buttons-race">
						<a href="/circuits" title="Go to Circuits Information">
							Circuits
							<Icon data={externalLink} />
						</a>
						<a href="/drivers" title="Go to Drivers Information">
							Drivers
							<Icon data={externalLink} />
						</a>
					</div>
				</div>
				<div class="points-system">
					<h5>Points System</h5>
					<div class="points-list">
						<ul>
							<li><span>#01</span>25 points</li>
							<li><span>#02</span>18 points</li>
							<li><span>#03</span>15 points</li>
							<li><span>#04</span>12 points</li>
							<li><span>#05</span>10 points</li>
						</ul>
						<ul>
							<li><span>#06</span>8 points</li>
							<li><span>#07</span>6 points</li>
							<li><span>#08</span>4 points</li>
							<li><span>#09</span>2 points</li>
							<li><span>#10</span>1 points</li>
						</ul>
					</div>
				</div>
			</div>
			<div class="img-race">
				<img
					src="https://media.formula1.com/image/upload/content/dam/fom-website/sutton/2022/Bahrain/Sunday/1386703905.jpg"
					alt="F1 Race 1"
				/>
				<img
					src="https://media.formula1.com/image/upload/f_auto/q_auto/v1681909842/calendar.jpg.transform/9col/image.jpg"
					alt="F1 Race 2"
				/>
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
		font-family: "Space Grotesk", monospace;
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
		font-family: "Space Grotesk", monospace;
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

	/* How it works Intro Section  */
	#howitworks {
		display: flex;
		flex-direction: column;
		align-items: start;
		gap: 4rem;
	}

	#howitworks .how-intro {
		display: flex;
		flex-direction: row;
		align-items: start;
		gap: 4rem;
	}
	#howitworks .how-intro img {
		flex: 1;
		width: 30vw;
		height: auto;
		border-radius: 0.5rem;
	}
	#howitworks .how-intro .how-intro-desc {
		display: flex;
		flex-direction: column;
		align-items: center;
		flex: 1;
		font-weight: 500;
		gap: 1rem;
	}
	#howitworks .how-intro .how-intro-desc h3 {
		font-size: 4rem;
		text-align: center;
		font-weight: 700;
		font-family: 'Space Grotesk', monospace;
		line-height: 1;
		margin-bottom: 1rem;
		color: hsl(80, 100%, 59%);
	}
	.how-intro-desc p {
		font-size: 1.0625rem;
		margin-bottom: 0.5rem;
	}
	.days-of-races {
		display: flex;
		flex-direction: column;
		align-items: start;
		gap: 0.75rem;
	}
	.days-of-races li {
		list-style-type: none;
		font-size: 1.2rem;
		display: flex;
		align-items: center;
	}

	.days-of-races li:nth-child(1) {
		margin-bottom: 0.5rem;
		font-size: 1.3rem;
		font-weight: 700;
	}
	.days-of-races li span:nth-child(1) {
		width: 2.5rem;
		aspect-ratio: 1/1;
		display: grid;
		place-items: center;
		border-radius: 100%;
		background-color: #ff1801;
		font-weight: 900;
		font-size: 1.5rem;
		margin-right: 1rem;
		border: 2px solid hsl(0, 0%, 95%);
	}

	.days-of-races li span:nth-child(2) {
		margin-left: 1rem;
		font-size: 1.5rem;
		font-weight: 800;
		color: #ff716f;
	}

	/* How it works Free Practice & Qualifying Sections */
	.practice-quali {
		display: flex;
		align-items: start;
		gap: 4rem;
	}
	.free-practice,
	.qualifying {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: start;
		gap: 1rem;
	}

	.free-practice .fp-sessions img,
	.qualifying .quali-sessions img {
		aspect-ratio: 4/3;
		width: 20vw;
		border-radius: 1rem;
		transition: all 350ms ease-in-out;
	}
	.free-practice .fp-sessions img:hover,
	.qualifying .quali-sessions img:hover {
		scale: 1.05;
	}

	.main-title {
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
	}
	.main-title h4 {
		font-size: 4rem;
		line-height: 1;
		font-family: 'Space Grotesk', monospace;
		color: hsl(80, 100%, 59%);
	}
	.main-title p {
		font-size: 1.5rem;
	}

	.fp-quali p {
		font-size: 1.05rem;
		font-weight: 600;
	}

	.fp-sessions,
	.quali-sessions {
		display: flex;
		align-items: start;
		justify-content: space-between;
		gap: 2rem;
	}
	.fp-sessions ul,
	.quali-sessions ul {
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
		list-style-type: none;
	}
	.fp-sessions ul li,
	.quali-sessions ul li {
		display: flex;
		align-items: center;
		gap: 2rem;
	}
	.fp-sessions ul li span,
	.quali-sessions ul li span {
		width: 2rem;
		aspect-ratio: 1/1;
		display: grid;
		place-items: center;
		background-color: hsl(80, 100%, 34%);
		border: 2px solid hsl(0, 0%, 95%);
		font-weight: 900;
		font-size: 1.25rem;
		border-radius: 100%;
	}

	/* MAIN RACE SECTION  */
	.main-race {
		display: flex;
		flex-direction: row;
		align-items: start;
		gap: 2rem;
		margin-bottom: 4rem;
	}
	.layout-race {
		display: flex;
		flex: 2;
		align-items: start;
		flex-direction: row;
	}

	.main-race-desc {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		flex: 1;
	}
	.main-race-desc p {
		font-weight: 500;
	}
	.main-race-desc .buttons-race {
		display: flex;
		align-items: center;
		gap: 2rem;
		margin-top: 1rem;
	}
	.buttons-race a {
		display: flex;
		align-items: center;
		gap: 1rem;
		font-size: 1.2rem;
		padding: 0.75rem 1.5rem;
		border-radius: 0.5rem;
		box-shadow: 1px 1px 8px hsla(0, 0%, 6%, 0.75);
		transition: all 350ms ease-in-out;
	}
	.buttons-race a:nth-child(1) {
		background-color: #d90b0b;
	}
	.buttons-race a:nth-child(2) {
		background-color: #bf9663;
	}
	.buttons-race a:nth-child(1):hover {
		scale: 1.025;
		background-color: #e92020;
	}
	.buttons-race a:nth-child(2):hover {
		scale: 1.025;
		background-color: #e8b980;
	}

	.points-system {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1rem;
	}
	.points-system h5 {
		font-size: 2rem;
		font-family: 'Space Grotesk', monospace;
		color: hsl(80, 100%, 59%);
		font-weight: 400;
	}
	.points-list {
		display: flex;
		gap: 2rem;
	}
	.points-list ul {
		list-style-type: none;
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	.points-list ul li {
		display: flex;
		flex-direction: row;
		align-items: center;
		font-size: 1.25rem;
	}
	.points-list ul li span {
		width: 4rem;
		height: 2.5rem;
		background-color: hsl(80, 100%, 34%);
		font-size: 1.25rem;
		font-weight: 700;
		display: grid;
		place-items: center;
		border-radius: 0.5rem;
		border: 2px solid hsl(0, 0%, 95%);
		margin-right: 0.5rem;
	}

	.img-race {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1rem;
	}
	.img-race img {
		width: 30vw;
		aspect-ratio: 4/1.5;
		object-fit: cover;
		object-position: bottom;
		border-radius: 0.5rem;
		opacity: 0.9;
		transition: all 350ms ease-in-out;
	}
	.img-race img:hover {
		opacity: 1;
		scale: 1.05;
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
		#howitworks .how-intro {
			flex-direction: column;
			align-items: center;
			gap: 2rem;
		}
		#howitworks .how-intro img {
			width: 80vw;
		}
		.practice-quali {
			flex-direction: column;
			align-items: center;
		}
		.free-practice .fp-sessions img,
		.qualifying .quali-sessions img {
			aspect-ratio: 21/9;
			width: 60vw;
			object-fit: cover;
			object-position: bottom;
		}

		.main-race {
			flex-direction: column;
			align-items: center;
		}
		.img-race {
			margin-top: 2rem;
			flex-direction: row;
		}
		.img-race img {
			width: 40vw;
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

		#howitworks {
			margin-inline: 0.5rem;
		}
		.free-practice .fp-sessions img,
		.qualifying .quali-sessions img {
			width: 80vw;
		}

		.fp-sessions,
		.quali-sessions {
			display: flex;
			flex-direction: column;
			gap: 2rem;
		}

		.layout-race {
			flex-direction: column;
			align-items: center;
			gap: 3rem;
		}
		.img-race {
			flex-direction: column;
		}
		.img-race img {
			width: 80vw;
		}
	}
</style>
