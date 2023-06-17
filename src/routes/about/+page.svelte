<script>
	import Icon from 'svelte-awesome';
    import githubSquare from 'svelte-awesome/icons/githubSquare';
    import codepen from 'svelte-awesome/icons/codepen';
    import externalLink from 'svelte-awesome/icons/externalLink';
</script>

<div class="main-page">
	<section class="about">
		<div class="description">
			<h1>What is This Website ?</h1>
			<p>
				This website is a project for my 2nd Semester Web App Development course at school. Since I
				am a Formula One fan, I dedicated my time to make the simplest also easiest way to
				understand what Formula One is about, especially its circuits, drivers, and teams from all
				over the world that are competing to win the World Championship
			</p>
		</div>
		<p>
			So, thank you so much to all of you that visited this website. I am very grateful with the
			result and you can learn more about me through the links below
		</p>
		<ul class="links">
			<li><a href="https://github.com/MatthewEvan" target="_blank"><Icon data={githubSquare} scale={1.5}/></a></li>
            <li><a href="https://codepen.io/MattXA25" target="_blank"><Icon data={codepen} scale={1.5}/></a></li>
            <li><a href="https://mulai-kerja-id.netlify.app/" target="_blank"><Icon data={externalLink} scale={1.5}/><p>MulaiKerja.id</p></a></li>
            <li><a href="https://cv-svelte-spongebob-matt.web.app/" target="_blank"><Icon data={externalLink} scale={1.5}/><p>Spongebob CV</p></a></li>
		</ul>
	</section>
	<section class="message">
		<h2>A Thank You Note</h2>
		<p>
			Thank you <b>Ko Moses</b> for all the things that you've done and taught me in the whole two semester
			of Web App Development. I am really grateful to be one of your students, because I can finally
			understand what it takes to make a website and designing it. I've learned how to correctly design
			and layout a website from the scratch, whether using Vanilla HTML, CSS, and JS or using a framework
			like Svelte for this website. Unfortunately, this extracurricular has come to an end. I'm sorry
			for all the minor inconveniences that I had done and I hope that we could meet again someday.
		</p>
        <h3> Thank you so much, Ko 🙏- Matthew</h3>
	</section>
</div>

<style>
	.main-page {
		display: flex;
		align-items: start;
		flex-direction: row;
		gap: 4rem;
		margin: 2rem 4rem 4rem;
		color: white;
	}
    a {
        color: white;
    }

    .about {
        flex: 1;
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }
    .description {
        display: flex;
        flex-direction: column;
        gap: 0.75rem;
    }
    .about .description h1 {
        font-size: 2.25rem;
        font-family: "Space Grotesk", monospace;
        font-weight: 700;
        line-height: 1;
    }
    .about .description p {
        padding-top: 1.25rem;
        border-top: solid 2px hsl(0, 0%, 95%);
        text-align: justify;
        font-size: 1.1rem;
        font-weight: 500;
    }
    .about > p {
        font-family: "Space Grotesk", monospace;
        font-weight: 400;
        line-height: 1.25;
    }

    .about ul {
        display: flex;
        align-items: center;
        gap: 1.5rem;
        list-style-type: none;
        margin-top: 1rem;
    }
    .about .links li a {
        display: flex;
        align-items: center;
        gap: 0.5rem;
        opacity: 0.8;
        transition: all 250ms ease-in-out
    }
    .about .links li a:hover {
        opacity: 1;
    }

    .message {
        flex: 1;
        display: flex;
        flex-direction: column;
        align-items: start;
        gap: 0.75rem;
        margin-bottom: 4rem;
    }
    .message h2 {
        font-size: 2.25rem;
        font-family: "Space Grotesk", monospace;
        font-weight: 700;
        line-height: 1;
    }
    .message p {
        padding-top: 1.25rem;
        border-top: solid 2px hsl(0, 0%, 95%);
        text-align: justify;
        font-size: 1.1rem;
        font-weight: 400;
        line-height: 1.4;
    }
    .message h3 {
        font-size: 1.25rem;
    }

    @media screen and (max-width: 768px) {
        .main-page {
            flex-direction: column;
            align-items: center;
        }
    }
</style>
