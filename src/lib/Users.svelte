<script>
    let name = 'Mark';
    let color = 'red';
    function getNumber(){
        return Math.random()
    }

    setTimeout(()=>{
        color = 'blue';
        name = 'steve'
    },3000)

</script>

<h2>My name is {name}</h2>
<p>The number is {getNumber()}</p>
<p style="color:{color}">The sum is {1+10}</p>
