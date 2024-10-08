<script>
    import Users from "./lib/Users.svelte";
    let name;

    setTimeout(()=>{
        name = 'Miles'
    },3000)

</script>


<Users {name}/>






