<script>
    import { createEventDispatcher } from 'svelte'
    const dispatch = createEventDispatcher();

    let name;
    let age;

    function sayHello(){
        dispatch('handleHello',{
            name,
            age
        })
    }
</script>

<div class="container">
    <input type="text" bind:value={name}>
    <input type="number" bind:value={age}>
    <button on:click={sayHello}>Hello</button>
</div>