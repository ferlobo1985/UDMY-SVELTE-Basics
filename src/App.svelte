<script>
    import Users from "./lib/Users.svelte";
    let name;
</script>

<h1>the real name is: {name}</h1>
<Users bind:name/>