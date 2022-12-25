<script>
    /** @type {string} */
    let cardName;
    /** @type {string} */
    let accentColor;
    /** @type {number} */
    let currentValue;

    export { cardName, accentColor, currentValue };
</script>

<section>
    <div class="card-header">
        <h2>{cardName}</h2>
    </div>

    <p style="color: {accentColor}">{currentValue}</p>
</section>

<style>
    * {
        font-weight: 700;
    }

    section {
        width: 15rem;
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
        height: 100%;
        font-size: 4rem;
        display: flex;
        align-items: center;
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
