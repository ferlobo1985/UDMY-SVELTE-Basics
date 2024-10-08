<script>
    let newName = '';
    let names = ['Mike','Lisa','Steve'];
    function addName(){
        names = [...names,newName];
        newName = '';
    }

    let cars = [
        {id:1,brand:'Ford'},
        {id:2,brand:'Nissan'},
        {id:3,brand:'Chevy'}
    ]
</script>

<ul>
    {#each names as name, index (index+name) }
        <li>{index+1} - {name}</li>
    {/each}
</ul>
<input type="text" bind:value={newName}/>
<button on:click={addName}>Add name</button>

<hr/>
<ul>
    {#each cars as car (car.id)}
        <li>{car.brand}</li>
    {/each}
</ul>