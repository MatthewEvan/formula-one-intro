<script>
    import MaxVerstappen from "$assets/drivers-page/MaxVerstappen.png";
    import SergioPerez from "$assets/drivers-page/SergioPerez.png";
    import FernandoAlonso from "$assets/drivers-page/FernandoAlonso.png";
    import LanceStroll from "$assets/drivers-page/LanceStroll.png";
    import LewisHamilton from "$assets/drivers-page/LewisHamilton.png";
    import GeorgeRussell from "$assets/drivers-page/GeorgeRussell.png";
    import CharlesLeclerc from "$assets/drivers-page/CharlesLeclerc.png";
    import CarlosSainz from "$assets/drivers-page/CarlosSainz.png";
    import EstebanOcon from "$assets/drivers-page/EstebanOcon.png";
    import PierreGasly from "$assets/drivers-page/PierreGasly.png";
    import LandoNorris from "$assets/drivers-page/LandoNorris.png";
    import OscarPiastri from "$assets/drivers-page/OscarPiastri.png";
    import ValtteriBottas from "$assets/drivers-page/ValtteriBottas.png";
    import ZhouGuanyu from "$assets/drivers-page/ZhouGuanyu.png";
    import KevinMagnussen from "$assets/drivers-page/KevinMagnussen.png";
    import NicoHulkenberg from "$assets/drivers-page/NicoHulkenberg.png";
    import YukiTsunoda from "$assets/drivers-page/YukiTsunoda.png";
    import NyckDeVries from "$assets/drivers-page/NyckDeVries.png";
    import AlexanderAlbon from "$assets/drivers-page/AlexanderAlbon.png";
    import LoganSargeant from "$assets/drivers-page/LoganSargeant.png";

    let drivers = [
        { number: "1", color: "#3671C6", id1: "Max", id2:"Verstappen", image: MaxVerstappen, team: "Red Bull Racing",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Flag_of_the_Netherlands.svg/800px-Flag_of_the_Netherlands.svg.png"},
        { number: "11", color: "#3671C6", id1: "Sergio", id2:"Perez", image: SergioPerez, team: "Red Bull Racing",
        flag: "https://cdn.britannica.com/73/2573-004-29818847/Flag-Mexico.jpg"},

        { number: "14", color: "#358C75", id1: "Fernando", id2:"Alonso", image: FernandoAlonso, team: "Aston Martin F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/8/89/Bandera_de_Espa%C3%B1a.svg/1200px-Bandera_de_Espa%C3%B1a.svg.png"},
        { number: "18", color: "#358C75", id1: "Lance", id2:"Stroll", image: LanceStroll, team: "Aston Martin F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Flag_of_Canada_%28Pantone%29.svg/1200px-Flag_of_Canada_%28Pantone%29.svg.png"},

        { number: "44", color: "#6CD3BF", id1: "Lewis", id2:"Hamilton", image: LewisHamilton, team: "Mercedes AMG Petronas F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/f/f2/Flag_of_Great_Britain_%281707%E2%80%931800%29.svg"},
        { number: "63", color: "#6CD3BF", id1: "George", id2:"Russell", image: GeorgeRussell, team: "Mercedes AMG Petronas F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/f/f2/Flag_of_Great_Britain_%281707%E2%80%931800%29.svg"},

        { number: "16", color: "#F91536", id1: "Charles", id2:"Leclerc", image: CharlesLeclerc, team: "Ferrari F1 Team",
        flag: "https://cdn.britannica.com/50/2750-050-688E6E49/Flag-Monaco.jpg"},
        { number: "55", color: "#F91536", id1: "Carlos", id2:"Sainz", image: CarlosSainz, team: "Ferrari F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/8/89/Bandera_de_Espa%C3%B1a.svg/1200px-Bandera_de_Espa%C3%B1a.svg.png"},

        { number: "31", color: "#2293D1", id1: "Esteban", id2:"Ocon", image: EstebanOcon, team: "Alpine F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/en/thumb/c/c3/Flag_of_France.svg/1200px-Flag_of_France.svg.png"},
        { number: "10", color: "#2293D1", id1: "Pierre", id2:"Gasly", image: PierreGasly, team: "Alpine F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/en/thumb/c/c3/Flag_of_France.svg/1200px-Flag_of_France.svg.png"},

        { number: "4", color: "#F58020", id1: "Lando", id2:"Norris", image: LandoNorris, team: "McLaren F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/f/f2/Flag_of_Great_Britain_%281707%E2%80%931800%29.svg"},
        { number: "81", color: "#F58020", id1: "Oscar", id2:"Piastri", image: OscarPiastri, team: "McLaren F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/b/b9/Flag_of_Australia.svg/1024px-Flag_of_Australia.svg.png"},

        { number: "77", color: "#B6BABD", id1: "Valtteri", id2:"Bottas", image: ValtteriBottas, team: "Alfa Romeo F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/Flag_of_Finland.svg/1200px-Flag_of_Finland.svg.png"},
        { number: "24", color: "#B6BABD", id1: "Zhou", id2:"Guanyu", image: ZhouGuanyu, team: "Alfa Romeo F1 Team",
        flag: "https://cdn.britannica.com/90/7490-004-BAD4AA72/Flag-China.jpg"},

        { number: "20", color: "#C92D4B", id1: "Kevin", id2:"Magnussen", image: KevinMagnussen, team: "Haas F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/9/9c/Flag_of_Denmark.svg/640px-Flag_of_Denmark.svg.png"},
        { number: "12", color: "#C92D4B", id1: "Nico", id2:"Hulkenberg", image: NicoHulkenberg, team: "Haas F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/en/thumb/b/ba/Flag_of_Germany.svg/1200px-Flag_of_Germany.svg.png"},
        
        { number: "22", color: "#5E8FAA", id1: "Yuki", id2:"Tsunoda", image: YukiTsunoda, team: "AlphaTauri F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/en/thumb/9/9e/Flag_of_Japan.svg/1200px-Flag_of_Japan.svg.png"},
        { number: "21", color: "#5E8FAA", id1: "Nyck", id2:"De Vries", image: NyckDeVries, team: "AlphaTauri F1 Team",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Flag_of_the_Netherlands.svg/800px-Flag_of_the_Netherlands.svg.png"},

        { number: "23", color: "#37BEDD", id1: "Alexander", id2:"Albon", image: AlexanderAlbon, team: "Williams Racing",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Flag_of_Thailand.svg/320px-Flag_of_Thailand.svg.png"},
        { number: "2", color: "#37BEDD", id1: "Logan", id2:"Sargeant", image: LoganSargeant, team: "Williams Racing",
        flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/US_flag_51_stars.svg/2560px-US_flag_51_stars.svg.png"},
    ]
</script>

<div class="main-page">
	<section class="header">
		<h1>F1 Drivers 2023</h1>
		<p>
			Discover and support the drivers that are competing for the 2023's Formula One Championship
			Title, with the arrival of two newbies from Netherlands, Nyck De Vries, and from The United
			States, Logan Sargeant. Even though it's 2023, three drivers who holds World Driver's Champion
			titles are still competing to get more titles, who are Lewis Hamilton with 7 WDCs with Max
			Verstappen and Fernando Alonso with 2 WDCs
		</p>
	</section>
	<section class="drivers-grid">
        {#each drivers as driver}
            <div class="driver-tile">
                <div class="driver-heading">
                    <p class="racing-number">{driver.number}</p>
                    <span style="background-color: {driver.color}"></span>
                    <div class="name">
                        <p>{driver.id1}</p>
                        <p>{driver.id2}</p>
                    </div>
                    <img src={driver.flag} alt="Driver's Nationality">
                </div>
                <div class="driver-team">
                    <p>{driver.team}</p>
                </div>
                <img src={driver.image} alt={driver.id2}>
            </div>
        {/each}
    </section>
</div>

<style>
	.main-page {
		display: flex;
		align-items: center;
		flex-direction: column;
		gap: 4rem;
		margin: 1rem 4rem 4rem;
		color: white;
	}

    .header {
        padding: 1.5rem 1.5rem 1rem 0;
        border-radius: 0 1rem 0 0;
        border-top: 3px solid #FF1801;
        border-right: 8px solid #FF1801;
        display: flex;
        flex-direction: column;
        align-items: start;
        gap: 1rem;
    }
    .header h1 {
        font-size: 4.5rem;
        font-family: "Space Mono", monospace;
        font-weight: 700;
        line-height: 1;
    }
    .header p {
        font-size: 1.2rem;
        font-family: "Space Mono", monospace;
        font-weight: 400;
        line-height: 1.2;
    }

    .drivers-grid {
        display: grid;
        grid-template-columns: repeat(4, minmax(0, 1fr));
        gap: 3rem;
        margin-bottom: 4rem;
    }
    .driver-tile {
        padding: 1rem;
        border-radius: 0 1rem 0 0;
        border-top: 2px solid hsl(0, 0%, 95%);
        border-right: 4px solid hsl(0, 0%, 95%);
        display: flex;
        flex-direction: column;
        align-items: start;
        gap: 1rem;
    }
    .driver-heading {
        display: flex;
        align-items: center;
        gap: 1rem;
        padding-bottom: 1rem;
        border-bottom: 2px solid hsl(0, 0%, 95%);
    }
    .racing-number {
        font-size: 2.5rem;
        font-family: "Space Mono", monospace;
        font-weight: 700;
        line-height: 1; 
    }

    .driver-heading span {
        width: 0.5rem;
        height: 2.5rem;
        border-radius: 0.2rem;
        background-color: white;
    }
    .driver-heading .name {
        display: flex;
        flex-direction: column;
    }
    .name p:nth-child(1) {
        font-size: 1.125rem;
        font-weight: 400;
    }
    .name p:nth-child(2){
        font-size: 1.25rem;
        font-weight: 800;
    }
    .driver-heading > img {
        width: 3rem;
        aspect-ratio: 3/2;
        object-fit: cover;
        border-radius: 0.25rem;
    }
    .driver-team {
        margin-left: 1rem;
        font-weight: 600;
    }
    .driver-team p {
        font-size: 1.3rem;
    }
    .driver-tile > img {
        width: 15vw;
    }

    @media screen and (max-width: 1024px) {
        .main-page {
            margin: 1rem 2rem 2rem;
        }

        .drivers-grid {
            grid-template-columns: repeat(2, minmax(0, 1fr));
        }
        .driver-tile > img {
            width: 35vw;
        }
    }

    @media screen and (max-width: 768px) {
        .header h1 {
            font-size: 3.5rem;
        }

        .drivers-grid {
            grid-template-columns: minmax(0, 1fr);
        }
        .driver-tile > img {
            width: 65vw;
        }
    }
</style>
