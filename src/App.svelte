<script>
    import Users from "./lib/Users.svelte";
    let users = false;
</script>

{#if users}
    <Users/>
{/if}

<button on:click={()=> users = !users}>
    Show and hide
</button>



