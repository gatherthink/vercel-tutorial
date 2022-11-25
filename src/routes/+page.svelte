



<script>
    let quantity = 0;

    function addToCart() {
        quantity = ++quantity
    }

</script>

<h1>Welcome to SvelteKit</h1>
<h2>There are {quantity} in the shopping cart</h2>

<button on:click={addToCart}>
    Add To cart
</button>

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>