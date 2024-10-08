<script>
    import Users from "./lib/Users.svelte";
    function handleHello(e){
        console.log(e)
        console.log(`hello ${e.detail.name} of age ${e.detail.age}`)
    }
</script>


<Users on:handleHello={handleHello}/>

