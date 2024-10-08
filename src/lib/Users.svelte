<script>
    import { onMount, onDestroy } from 'svelte'

    onMount(()=>{
        console.log('Users COMP, MOUNTED');

        // return()=>{
        //     console.log('COMP unmounted')
        // }
    })

    onDestroy(()=>{
        console.log('COMP unmounted')
    })

</script>


<div class="container">
  <h1>Users component</h1>
</div>