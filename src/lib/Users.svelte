<script>
    let name = 'Jake';
    $: message = name + ' - Joined the chat'

    let number = 0;
    let mult = 2;
    function addNumber(value,mult){
        return value * mult;
    }
    $: total = addNumber(number,mult)

    $: {
        console.log(mult)
        alert(`The mult is now: ${mult}`)
    }

</script>


<div class="container">
    <i>Initial name:{name}</i>
    <h2>{message}</h2>
    <hr/>
    <button on:click={()=>name='Mike'}>Change the name</button>

    <hr/>
    <p>Total:{total}</p>
    <button on:click={()=>number++}>Add number</button>
    <input type="number" bind:value={mult}>

</div>