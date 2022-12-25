<script>
    import Card from "./Card.svelte";
    import BigCard from "./BigCard.svelte";

    const red = "#EB5757";
    const blue = "#2D9CDB";
    const green = "#27AE60";
    const yellow = "#F2C94C";
</script>

<svelte:head>
	<title>Dashboard</title>
	<meta name="description" content="Dashboard" />
</svelte:head>

<section>
    <div class="dashboard-header">
        <h1>Dashboard</h1>
    </div>

    <div class="stats-cards">
        <Card cardName="In queue"      accentColor={yellow} currentValue={83}/>
        <Card cardName="In work"       accentColor={blue}   currentValue={39}/>
        <Card cardName="Done"          accentColor={green}  currentValue={172}/>
        <Card cardName="Rejected"      accentColor={red}    currentValue={61}/>
    </div>

    <BigCard cardName="General Stats" accentColor={green}  currentValue={5}/>
</section>

<style>
    section {
        display: flex;
        align-items: center;
		justify-content: center;
        flex-direction: column;
        width: 100%;
	}
    
    .stats-cards {
        display: flex;
        flex-direction: row;
        gap: 20px;
    }
</style>
