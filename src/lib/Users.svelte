<script>
let promisePosts = getPosts();
async function getPosts(){
    const response = await fetch('https://jsonplaceholder.typicode.com/posts');
    const posts = await response.json();

    // throw new Error('Something wrong')
    return posts;
}
</script>

{#await promisePosts}
    <p>Loading...</p>
{:then posts } 
    
    {#each posts as post (post.id)}
        <p>{post.title}</p>
        <hr/>
    {/each}

{:catch error}
    <p>{error}</p>
{/await}
