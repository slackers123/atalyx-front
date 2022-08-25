<script>
    import { goto } from "$app/navigation";
    export let src = "amonkstale.png";
    export let title = "A Monks Tale"
    export let link = "/games/a-monks-tale";
</script>

<div class="cont" on:click={() => goto(link)}>
    <img {src} alt="{title} Logo">
    <h3>{title}</h3>
</div>


<style>

    .cont {
        width: 100%;
        margin-right: 1rem;
    }

    img {
        width: 100%;
    }
    h3 {
        font-size: 2rem;
    }
</style>