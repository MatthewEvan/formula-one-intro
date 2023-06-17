<script>
	import Icon from 'svelte-awesome';
	import mapMarker from 'svelte-awesome/icons/mapMarker';

    let circuits = [
        {number: "1", id: "Formula 1 Gulf Air Bahrain Grand Prix", location: "Bahrain", imgID: "Bahrain_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flag_of_Bahrain_%28bordered%29.svg/2560px-Flag_of_Bahrain_%28bordered%29.svg.png"},
        {number: "2", id: "Formula 1 STC Saudi Arabian Grand Prix", location: "Saudi Arabia", imgID: "Saudi_Arabia_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/0d/Flag_of_Saudi_Arabia.svg/1280px-Flag_of_Saudi_Arabia.svg.png"},
        {number: "3", id: "Formula 1 Rolex Australian Grand Prix", location: "Australia", imgID: "Australia_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/b/b9/Flag_of_Australia.svg/1024px-Flag_of_Australia.svg.png"},
        {number: "4", id: "Formula 1 Azerbaijan Grand Prix", location: "Azerbaijan", imgID: "Baku_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/d/dd/Flag_of_Azerbaijan.svg"},
        {number: "5", id: "Formula 1 Crypto.com Miami Grand Prix", location: "Miami", imgID: "Miami_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/US_flag_51_stars.svg/2560px-US_flag_51_stars.svg.png"},
        {number: "6", id: "Formula 1 Grand Prix de Monaco", location: "Monaco", imgID: "Monoco_Circuit.png", 
        flagID: "https://cdn.britannica.com/50/2750-050-688E6E49/Flag-Monaco.jpg"},
       
        {number: "7", id: "Formula 1 AWS Gran Premio de España", location: "Spain", imgID: "Spain_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/8/89/Bandera_de_Espa%C3%B1a.svg/1200px-Bandera_de_Espa%C3%B1a.svg.png"},
        {number: "8", id: "Formula 1 Pirelli Grand Prix du Canada", location: "Canada", imgID: "Canada_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Flag_of_Canada_%28Pantone%29.svg/1200px-Flag_of_Canada_%28Pantone%29.svg.png"},
        {number: "9", id: "Formula 1 Rolex Grosser Preis Von Österreich", location: "Austria", imgID: "Austria_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/Flag_of_Austria.svg/255px-Flag_of_Austria.svg.png"},
        {number: "10", id: "Formula 1 Aramco British Grand Prix", location: "Great Britain", imgID: "Great_Britain_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/f/f2/Flag_of_Great_Britain_%281707%E2%80%931800%29.svg"},
        {number: "11", id: "Formula 1 Qatar Airways Hungarian Grand Prix", location: "Hungary", imgID: "Hungary_Circuit.png", 
        flagID: "https://cdn.britannica.com/55/1455-004-5897143C/Flag-Hungary.jpg"},
        {number: "12", id: "Formula 1 MSc Cruises Belgian Grand Prix", location: "Belgium", imgID: "Belgium_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/65/Flag_of_Belgium.svg/900px-Flag_of_Belgium.svg.png"},
       
        {number: "13", id: "Formula 1 Heineken Dutch Grand Prix", location: "Netherlands", imgID: "Netherlands_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Flag_of_the_Netherlands.svg/800px-Flag_of_the_Netherlands.svg.png"},
        {number: "14", id: "Formula 1 Pirelli Gran Premio D'Italia 2023", location: "Italy", imgID: "Italy_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/en/thumb/0/03/Flag_of_Italy.svg/800px-Flag_of_Italy.svg.png"},
        {number: "15", id: "Formula 1 Singapore Airlines Singapore Grand Prix", location: "Singapore", imgID: "Singapore_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Flag_of_Singapore.svg/1200px-Flag_of_Singapore.svg.png"},
        {number: "16", id: "Formula 1 Lenovo Japanese Grand Prix", location: "Japan", imgID: "Japan_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/en/thumb/9/9e/Flag_of_Japan.svg/1200px-Flag_of_Japan.svg.png"},
        {number: "17", id: "Formula 1 Qatar Airways Qatar Grand Prix", location: "Qatar", imgID: "Qatar_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/3/3e/Flag_of_Qatar_%283-2%29.svg/2560px-Flag_of_Qatar_%283-2%29.svg.png"},
        {number: "18", id: "Formula 1 Lenovo United States Grand Prix", location: "United States", imgID: "USA_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/US_flag_51_stars.svg/2560px-US_flag_51_stars.svg.png"},
       
        {number: "19", id: "Formula 1 Gran Premio de La Ciudad de México", location: "Mexico", imgID: "Mexico_Circuit.png", 
        flagID: "https://cdn.britannica.com/73/2573-004-29818847/Flag-Mexico.jpg"},
        {number: "20", id: "Formula 1 Rolex Grande Prêmio de São Paulo", location: "Brazil", imgID: "Brazil_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Flag_of_Brazil.svg/1024px-Flag_of_Brazil.svg.png"},
        {number: "21", id: "Formula 1 Heineken Silver Las Vegas Grand Prix", location: "Las Vegas, USA", imgID: "Las_Vegas_Circuit.png", 
        flagID: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/US_flag_51_stars.svg/2560px-US_flag_51_stars.svg.png"},
        {number: "22", id: "Formula 1 Etihad Airways Abu Dhabi Grand Prix", location: "Abu Dhabi, UAE", imgID: "Abu_Dhabi_Circuit.png", 
        flagID: "https://cdn.britannica.com/82/5782-050-8A763A9A/Flag-United-Arab-Emirates.jpg"}
    ]
</script>

<div class="main-page">
	<section class="heading">
		<h1>F1 Circuits 2023</h1>
		<p>
			All the circuits that are used for F1'S 2023 World Championship all across the world. From the
			East to the West, all circuits are iconic with its own challenging parts, fans, and locations.
			One of the most famous place, Las Vegas is said to be on the calendar of 2023's Formula One
			Championship as the second last grand prix before Abu Dhabi Grand Prix
		</p>
	</section>
	<section class="map-grid">
        {#each circuits as circuit}
            <div class="circuit-tile">
                <div class="circuit-heading">
                    <p class="number">{circuit.number}</p>
                    <span></span>
                    <p class="circuit-name">{circuit.id}</p>
                </div>
                <div class="location">
                    <Icon data={mapMarker} scale={2}/>
                    <img src="{circuit.flagID}" alt="">
                    <p>{circuit.location}</p>
                </div>
                <img src="https://media.formula1.com/image/upload/content/dam/fom-website/2018-redesign-assets/Circuit%20maps%2016x9/{circuit.imgID}" alt="{circuit.location} Circuit">
            </div>
        {/each}
    </section>
</div>

<style>
	.main-page {
		margin: 1rem 4rem 4rem;
		color: white;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 4rem;
	}

	.heading {
		padding: 1.5rem 2rem 1.5rem 0rem;
		display: flex;
		flex-direction: column;
		align-items: start;
		border-right: 8px solid #ff1801;
		border-top: 8px solid #ff1801;
		border-radius: 0rem 2rem 0rem 0rem;
		gap: 1rem;
	}
	.heading h1 {
		font-size: 5rem;
		font-family: 'Space Grotesk', monospace;
		font-weight: 700;
		line-height: 1;
	}
    .heading p {
        font-size: 1.2rem;
        font-family: 'Space Grotesk', monospace;
		font-weight: 400;
		line-height: 1.2;
    }

    .map-grid {
        display: grid;
        grid-template-columns: repeat(4, minmax(0, 1fr));
        gap: 4rem;
        margin-bottom: 4rem;
    }
    .circuit-tile {
        padding: 1rem;
        border-top: 2px solid hsl(0, 0%, 95%);
        border-left: 6px solid hsl(0, 0%, 95%);
        border-radius: 1rem 0 0 0;
        display: flex;
        flex-direction: column;
        gap: 1.5rem;
        align-items: start;
    }
    .circuit-heading {
        display: flex;
        align-items: center;
        gap: 1rem;
    }
    .circuit-heading .number {
        font-size: 2.5rem;
        font-family: 'Space Grotesk', monospace;
		font-weight: 700;
		line-height: 1;
    }
    .circuit-heading span {
        background-color: #FF1801;
        width: 0.5rem;
        height: 2.5rem;
        border-radius: 0.25rem;
    }
    .circuit-heading p {
        font-size: 1.25rem;
        font-family: "Space Grotesk", monospace;
        line-height: 1.15;
    }

    .location {
        display: flex;
        align-items: center;
        gap: 1.25rem;
        margin-left: 1rem;
    }
    .location img {
        width: 4rem;
        border-radius: 0.5rem;
        aspect-ratio: 3/2;
        object-fit: cover;
    }
    .location p {
        font-size: 1.25rem;
        font-weight: 700;
    }

    .circuit-tile > img {
        width: 20vw;
        margin-top: 2rem;
    }


	@media screen and (max-width: 1024px) {
		.main-page {
			margin: 1rem 4rem 4rem;
		}

        .map-grid {
          display: grid;
          grid-template-columns: repeat(2, minmax(0, 1fr));
          gap: 4rem;
        }
        .circuit-tile > img {
            width: 40vw;
            margin-top: 2rem;
        }
	}

	@media screen and (max-width: 768px) {
		.main-page {
			margin: 1rem 2rem 4rem;
		}
        .heading h1 {
            font-size: 4rem;
        }

        .map-grid {
          display: grid;
          grid-template-columns: minmax(0, 1fr);
        }
        .circuit-tile > img {
            width: 80vw;
            margin-top: 2rem;
        }
	}
</style>
