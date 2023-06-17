<script>
    import RedBullLogo from "$assets/teams-page/RedBullLogo.png"
    import RedBullImage from "$assets/teams-page/RedBullTeam.png"
    import MercedesLogo from "$assets/teams-page/MercedesLogo.png"
    import MercedesImage from "$assets/teams-page/MercedesTeam.png"
    import FerrariLogo from "$assets/teams-page/FerrariLogo.png"
    import FerrariImage from "$assets/teams-page/FerrariTeam.png"
    import AstonMartinLogo from "$assets/teams-page/AstonMartinLogo.png"
    import AstonMartinImage from "$assets/teams-page/AstonMartinTeam.png"
    import AlpineLogo from "$assets/teams-page/AlpineLogo.png"
    import AlpineImage from "$assets/teams-page/AlpineTeam.png"
    import McLarenLogo from "$assets/teams-page/McLarenLogo.png"
    import McLarenImage from "$assets/teams-page/McLarenTeam.png"
    import AlfaRomeoLogo from "$assets/teams-page/AlfaRomeoLogo.png"
    import AlfaRomeoImage from "$assets/teams-page/AlfaRomeoTeam.png"
    import HaasLogo from "$assets/teams-page/HaasLogo.png"
    import HaasImage from "$assets/teams-page/HaasTeam.png"
    import AlphaTauriLogo from "$assets/teams-page/AlphaTauriLogo.png"
    import AlphaTauriImage from "$assets/teams-page/AlphaTauriTeam.png"
    import WilliamsLogo from "$assets/teams-page/WilliamsLogo.png"
    import WilliamsImage from "$assets/teams-page/WilliamsTeam.png"

	let teams = [
        { number: "1", color: "#3671C6", id: "Red Bull", logo: RedBullLogo, driver1: "Max Verstappen", driver2: "Sergio Perez", img: RedBullImage},
        { number: "2", color: "#358C75", id: "Aston Martin", logo: AstonMartinLogo, driver1: "Fernando Alonso", driver2: "Lance Stroll", img: AstonMartinImage},
        { number: "3", color: "#6CD3BF", id: "Mercedes", logo: MercedesLogo, driver1: "Lewis Hamilton", driver2: "George Russell", img: MercedesImage},
        { number: "4", color: "#F91536", id: "Ferrari", logo: FerrariLogo, driver1: "Charles Leclerc", driver2: "Carlos Sainz", img: FerrariImage},
        { number: "5", color: "#2293D1", id: "Alpine", logo: AlpineLogo, driver1: "Esteban Ocon", driver2: "Pierre Gasly", img: AlpineImage},
        { number: "6", color: "#F58020", id: "McLaren", logo: McLarenLogo, driver1: "Lando Norris", driver2: "Oscar Piastri", img: McLarenImage},
        { number: "7", color: "#B6BABD", id: "Haas", logo: HaasLogo, driver1: "Kevin Magnussen", driver2: "Nico Hulkenberg", img: HaasImage},
        { number: "8", color: "#C92D4B", id: "Alfa Romeo", logo: AlfaRomeoLogo, driver1: "Zhou Guanyu", driver2: "Valtteri Bottas", img: AlfaRomeoImage},
        { number: "9", color: "#5E8FAA", id: "Alpha Tauri", logo: AlphaTauriLogo, driver1: "Yuki Tsunoda", driver2: "Nyck De Vries", img: AlphaTauriImage},
        { number: "10", color: "#37BEDD", id: "Williams", logo: WilliamsLogo, driver1: "Alexander Albon", driver2: "Logan Sargeant", img: WilliamsImage},
    ]
</script>

<div class="main-page">
	<section id="header">
		<h1>Formula One Teams 2023</h1>
		<p>
			Discover all the teams that are competing in the Formula One World Championship 2023 with
			different cars, drivers, and sponsors to win this year's championship. A total of 10 teams
			with the commitment of winning a race affected by a good starting position, strategy, and the
			performance of the car and driver.
		</p>
	</section>
    <section class="teams-grid">
        {#each teams as team} 
            <div class="team-tile">
                <div class="team-header">
                    <div class="number">
                        <p class="team-number">{team.number}</p>
                        <span style="background-color: {team.color}"></span>
                        <p class="team-title">{team.id}</p>
                        <img src={team.logo} alt={team.id}>
                    </div>
                </div>
                <div class="team-drivers">
                    <p>Drivers</p>
                    <div class="driver-names">
                        <p><span>&#8226;</span>{team.driver1}</p>
                        <p><span>&#8226;</span>{team.driver2}</p>
                    </div>
                </div>
                <img src={team.img} alt={team.id}>
            </div>
        {/each}
    </section>
</div>

<style>
	.main-page {
		color: white;
        margin: 2rem 3rem 4rem;
        display: flex;
        flex-direction: column;
        gap: 4rem;
	}
    #header {
        display: flex;
        flex-direction: column;
        align-items: start;
        margin-inline: 2rem;
        gap: 2rem;
    }
    #header h1 {
        font-size: 4.5rem;
        line-height: 1;
        padding: 1rem 2rem 1rem 0rem;
        border-right: 8px solid #FF1801;
        border-top: 8px solid  #FF1801;
        border-radius: 0rem 2rem 0rem 0rem;
        font-family: "Space Grotesk", monospace;
        font-weight: 700;
    }
    #header p {
        padding-bottom: 1rem;
        border-bottom: 4px solid hsl(0, 0%, 95%);
        font-family: "Space Grotesk", monospace;
        font-weight: 400;
        font-size: 1.1rem;
    }

    .teams-grid {
        display: grid;
        grid-template-columns: repeat(4, minmax(0, 1fr));
        gap: 2.5rem;
        margin-bottom: 4rem;
    }
    .team-tile {
        border-top: 2px solid hsl(0, 0%, 95%);
        border-right: 6px solid hsl(0, 0%, 95%);
        border-radius: 0 1rem 0 0;
        padding: 1rem;
        display: flex;
        flex-direction: column;
        align-items: start;
        gap: 0.5rem;
    }
    .team-header {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .number {
        display: flex;
        align-items: center;
        gap: 1rem;
    }
    .team-number {
        font-size: 2rem;
        font-family: "Space Grotesk", monospace;
        line-height: 1;
        font-weight: 700;
    }
    .number span {
        width: 0.5rem;
        height: 2.25rem;
        border-radius: 0.2rem;
    }
    .number .team-title {
        font-size: 1.5rem;
        font-family: "Space Grotesk", monospace;
        font-weight: 700;
        line-height: 1;
    }
    .team-header  .number img{
        width: 4rem;
        aspect-ratio: 1/1;
    }

    .team-drivers {
        display:flex;
        flex-direction: column;
        align-items: start;
        gap: 1rem;
    }
    .team-drivers > p {
        font-size: 2rem;
        font-weight: 800;
    }
    .team-drivers .driver-names {
        display: flex;
        align-items: center;
        gap: 1rem;
        font-weight: 600;
    }
    .driver-names p {
        display: flex;
        align-items: center;
        gap: 0.5rem;
        font-size: 1.15rem;
    }
    .team-tile > img {
        width: 18vw;
        margin-top: 1rem;
    }


    @media screen and (max-width: 1024px) {
        .main-page {
            margin: 2rem 2rem 4rem;
        }
        #header {
            margin-inline: 0.5rem;
        }

        .teams-grid {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 2.5rem;
        }
        .team-tile > img {
            width: 40vw;
            margin-top: 1rem;
        }
    }

     @media screen and (max-width: 768px) {
        .main-page {
            margin: 1rem 1.5rem 2rem;
        }
        
        .teams-grid {
            display: grid;
            grid-template-columns: minmax(0, 1fr);
            gap: 2.5rem;
        }
        .team-tile > img {
            width: 75vw;
            margin-top: 1rem;
        }
     }
</style>
