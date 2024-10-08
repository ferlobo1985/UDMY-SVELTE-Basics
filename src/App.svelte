<script>
    import Users from "./lib/Users.svelte";
</script>


<Users>
    <svelte:fragment slot="content">
        <p>Some content</p>
    </svelte:fragment>

    <!-- <svelte:fragment slot="footer">
        <p>Some footer content</p>
    </svelte:fragment> -->
</Users>

