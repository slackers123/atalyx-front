<script>
    export let src = "Toby Kogler.png";
    export let name = "Toby Kogler";
    export let roles = ["General Director", "Composer"];
</script>


<div class="content">
    <img {src} alt={name}>
    <h2>{name}</h2>
    {#each roles as role}
        <p>{role}</p>
    {/each}
</div>

<style>
    p {
        color: gray;
    }
</style>