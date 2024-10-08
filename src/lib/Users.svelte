<script>
    function saySomething(){
        alert('Hello there !!!')
    }
    function hanleInput(e){
        console.log(e.target.value,'input')
    }
    function handleForm(e){
        console.log('Done !!!')
    }
</script>

<form on:submit|preventDefault|stopPropagation={handleForm}>
    <input type="text" on:input={hanleInput}/>
    <button type="submit">Submit</button>
</form>

<button on:click={saySomething}>Say something</button>
