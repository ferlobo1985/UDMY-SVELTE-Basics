<script>
    import { beforeUpdate, afterUpdate } from 'svelte';
    export let name = 'Steve';

    beforeUpdate(()=>{
        console.log('BEFORE Update')
    })

    afterUpdate(()=>{
        console.log('AFTER Update')
    })

</script>


<div class="container">
    <h1>Users component</h1>
    <p>{name}</p>
    <hr/>
    <button on:click={()=> name="Mark"}>Update name</button>
</div>