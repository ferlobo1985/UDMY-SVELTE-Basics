<script>
    import Users from "./lib/Users.svelte";
    let name = 'Steve'

    setTimeout(()=>{
        name = 'Mark'
    },2000)

</script>

<Users username={name}/>