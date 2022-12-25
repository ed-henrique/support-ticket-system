<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<section>
	<h1>About this app</h1>

	<p>
		This is a demo app for a support ticket system, used in a broad range of business to handle both
		internal and external issues. 
	</p>
</section>

<style>
	h1, p {
        width: calc(60rem + 66px);
		display: flex;
        align-items: left;
        justify-content: left;
	}

	section {
		display: flex;
        align-items: center;
		justify-content: center;
        flex-direction: column;
        width: 100%;
	}
</style>
