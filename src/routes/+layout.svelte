<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;800&display=swap" rel="stylesheet">
    <title>Formula 1 Introduction</title>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
</svelte:head>

<slot/>

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
    }
    :global(a) {
        text-decoration: none;
    }
</style>