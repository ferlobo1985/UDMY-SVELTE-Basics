<script>
    let age = 20;
    let auth = true;
</script>

{#if !auth }
    <h2>you are not AUTH</h2>
{:else if age <= 10}
    <h2>You are too young</h2>
{:else}
    <h2>Welcome !!!</h2>
{/if}

<input type="number" bind:value={age}/>
<input type="checkbox" bind:checked={auth}/>