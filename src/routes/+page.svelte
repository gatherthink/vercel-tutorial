



<script>
    let quantity = 0;

    function addToCart() {
        quantity = ++quantity
        inventory = [... inventory, quantity];
    }

    let inventory = [1,2,3];
    let user = {name:'steph'};
    $: remaining = 10 - quantity;
    let price = 5;
    $: totalCost = 5*quantity;

</script>

<h1>Welcome to SvelteKit</h1>
<h2>There are {quantity} in the shopping cart</h2>
<h3>Inventory {inventory}</h3>
<h3>{user.name}</h3>
<h3>{totalCost}</h3>

<button on:click={addToCart}>
    Add To cart
</button>

<h4>Remaining inventory: {remaining} </h4>

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>