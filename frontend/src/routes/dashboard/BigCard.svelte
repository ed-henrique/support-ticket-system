<script lang="ts">
    let cardName: string;
    let accentColor: string;
    let currentValue: number;

    export { cardName, accentColor, currentValue };
</script>

<section>
    <div class="card-header">
        <h2>{cardName}</h2>
    </div>

    <div class="stats">
        <div class="stats-left">
            ADD BEAUTIFUL PIE CHART HERE
        </div>
        <div class="stats-right">
            <h3>Average Response Time:</h3>
            <p style="color: {accentColor}">{currentValue}h</p>
        </div>
    </div>

</section>

<style>
    * {
        font-weight: 700;
    }

    h3 {
        margin: 0;
    }

    section {
        margin-top: 20px;
        width: calc(60rem + 66px);
        height: 30rem;
        display: flex;
        align-items: center;
        flex-direction: column;
        overflow: hidden;
		text-transform: uppercase;
        border-radius: 1rem;
        border: 1px solid var(--border-color);
        background-color: var(--color-bg-secondary);
    }
    
    p {
        margin: 0;
        font-size: 4rem;
        display: flex;
        align-items: center;
    }

    .stats, .stats-left, .stats-right {
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: row;
    }
    
    .stats-left {
        color: red;
        font-weight: 400;
    }

    .stats-right {
        flex-direction: column;
        border-left: 1px solid var(--border-color);
    }

    .stats-right > p {
		text-transform: none;
    }

    .card-header {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        border-bottom: 1px solid #DDE7EC;
        background-color: var(--color-bg-card);
    }
</style>
