<script lang="ts">
	import MercedesW14 from '$assets/main-page/Mercedes-W14.png';
	import RedBullRB19 from '$assets/main-page/RedBull-RB19.png';

	import Icon from 'svelte-awesome';
	import angleDown from 'svelte-awesome/icons/angleDown';
	import lightbulbO from 'svelte-awesome/icons/lightbulbO';
	import tachometer from 'svelte-awesome/icons/tachometer';
</script>

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
                <svg class="f1-logo" width="10rem" viewBox="0 0 320 80" xmlns="http://www.w3.org/2000/svg">
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M45.2583 80L80.7417 45.575H80.7333C94.7167 32.0167 100.392 29.9583 127.058 29.9583H233.408L264.008 0H123.025C87.3333 0 77.2417 3.4 56.3083 24.1167L0 80H45.2583ZM127.7 34.7417H228.842L200.792 62.7917H128.225C114.925 62.7917 111.983 63.4167 105.383 70.0167L95.4 80H53.4333L84.4583 48.975C96.6417 36.8 100.842 34.7417 127.7 34.7417ZM320 0L239.783 80H190.175L270.175 0H320ZM267.183 77.4667C268.85 79.1583 270.95 80 273.475 80C276 80 278.075 79.1583 279.717 77.4833C281.358 75.8083 282.175 73.7333 282.175 71.2667C282.175 68.8 281.35 66.725 279.7 65.0333C278.05 63.3417 275.967 62.5 273.442 62.5C270.917 62.5 268.825 63.3417 267.167 65.0167C265.508 66.6917 264.675 68.7667 264.675 71.2333C264.675 73.7 265.508 75.775 267.183 77.4667ZM268.225 66.025C269.625 64.5917 271.358 63.875 273.425 63.875C275.5 63.875 277.233 64.5917 278.625 66.025C280.017 67.4583 280.717 69.2 280.717 71.25C280.717 73.3 280.017 75.0333 278.625 76.4583C277.225 77.8833 275.5 78.5917 273.425 78.5917C271.35 78.5917 269.617 77.875 268.225 76.4417C266.833 75.0083 266.133 73.275 266.133 71.2333C266.133 69.1917 266.833 67.4583 268.225 66.025ZM271.717 76.125V72.6917L271.725 72.7H273.683L275.342 76.1333H277.367L275.542 72.45C276.158 72.1667 276.592 71.8 276.85 71.3417C277.108 70.8833 277.233 70.1833 277.233 69.2417C277.233 68.3 276.917 67.5917 276.283 67.125C275.65 66.65 274.7 66.4167 273.442 66.4167H269.792V76.125H271.717ZM271.683 71.1833V67.9167H273.275C274.65 67.9167 275.333 68.4583 275.333 69.55C275.333 70.125 275.2 70.5417 274.933 70.8C274.675 71.0583 274.242 71.1833 273.642 71.1833H271.683Z"
					fill="#FF1801"
				/>
			    </svg>
            </a>
			<h1>
				<span>Formula One</span>, the pinnacle of motorsport where every race is a battle of
				technology and talent
			</h1>
			<p>
				Firstly held at the Silverstone Circuit on 13th of May 1950, Formula One has since been one
				of the most prestigious and innovative motorsport championship league with almost 171 teams
				and 774 drivers on 60+ different circuits around the world
			</p>
            <div class="discover-more">
                <a href="#content-overview">Discover More</a>
                <Icon data={angleDown} scale={1.5} style="color: hsl(0, 0%, 95%)"/>
            </div>
		</div>
		<img src={RedBullRB19} alt="Red Bull RB19" class="redbullrb19" />
	</div>
</section>

<style>
	/* #header #header #header */
	#header {
		margin: 2rem 4rem;
        position: relative;
        z-index: 5;
	}

	.circle-bg span{
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
        background-color: #ABF74F;
        opacity: 0.75;
    }
    .circle-bg span:nth-child(2) {
        width: 15vw;
        top: 5vh;
        left: 2vw;
        background-color: #7daff9;
        opacity: 0.75;
    } 
    .circle-bg span:nth-child(3) {
        width: 40vw;
        top: 8vh;
        left: 20vw;
        background-color: #c583ff;
        opacity: 0.75;
    }

	.main-header {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
		gap: 3rem;
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
        margin-bottom: 1rem;
	}
	.header-text h1 span {
		font-size: 4rem;
		font-weight: 900;
        background-image: linear-gradient(
            -135deg,
            #EA1B00,
            #F91D00,
            #F21C00,
            #CB1700,
            #A91400
        );
        -webkit-background-clip: text;
        background-clip: text;
        color: transparent;
	}
    .header-text p {
        color: #dadada;
        line-height: 1.15;
        font-weight: 500;
        font-size: 1.1rem;
        text-align: center;
        margin-bottom: 1rem;
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
        background-image: linear-gradient(
            -135deg,
            #EA1B00,
            #F91D00,
            #F21C00,
            #CB1700,
            #A91400
        );
        border-radius: 50rem;
        transition: all 350ms ease-in-out
    }
    .discover-more a:hover {
        background-image: linear-gradient(
            -90deg,
            #EA1B00,
            #F91D00,
            #F21C00,
            #CB1700,
            #A91400
        );
        box-shadow: 1px 1px 8px hsla(0, 0%, 6%, 0.75);
    }

    @media screen and (max-width: 1024px) {
        #header {
            margin: 2rem;
        }
        
        .main-header {
            gap: 1.5rem;
        }

        .mercedesw14, .redbullrb19 {
            height: 60vh;
        }
        .header-text h1 {
            font-size: 2.5rem;
        }
        .header-text h1 span {
            font-size: 3.5rem;
        }
    }

    @media screen and (max-width: 768px) {
        #header {
            margin: 4rem 2.5rem 2rem;
        }
        .main-header {
            flex-direction: column;
            gap: 0;
        }
        .mercedesw14, .redbullrb19 {
            display: none;
        }

    }
</style>
