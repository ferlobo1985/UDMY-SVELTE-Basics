<script>
   function myAction(node, args){
        node.style.color = args;
        node.innerHTML = 'Changed it';

        function handleClick(){
            console.log('Element clicked')
        }
        node.addEventListener('click',handleClick)

        return {
            destroy(){
                node.removeEventListener('click')
            }
        }
   }
</script>

<div class="container">
    <div use:myAction={'blue'}>Some element</div>
</div>