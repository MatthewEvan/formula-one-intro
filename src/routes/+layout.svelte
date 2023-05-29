<script>
    import Navbar from "$components/Navbar.svelte";
    import Footer from "$components/Footer.svelte";
</script>

<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;70;800;900&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
    <title>Formula 1 Introduction</title>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
</svelte:head>

<Navbar/>
<div class="readable-area">
    <slot/>
</div>
<Footer/>

<style>
    :global(*, *::before, *::after) {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-size: 14px;
        font-family: "Inter", sans-serif;
    }
    :global(html, body) {
        width: 100%;
        height: 100%;
        scroll-behavior: smooth;
        background-color: #101014;
    }
    :global(a) {
        text-decoration: none;
    }
    .readable-area {
        padding-top: 4.5rem;
    }
    @media screen and (max-width: 768px) {
        :global(*, *::before, *::after) {
            font-size: 12px;
        }
    }
</style>