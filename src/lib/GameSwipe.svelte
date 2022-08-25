<script>
    import { goto } from "$app/navigation";
    export let title = "A Monk's Tale";
    export let src = "sc1.png"
    export let link = "/games/a-monks-tale";
</script>

<div class="cont">
    <img {src} alt="{title} Thumbnail">
    <div class="title-btn">
        <h1>{title}</h1>
        <button on:click={() => {goto(link)}}> Explore </button>
    </div>
</div>

<style>
    button {
        margin-top: 2rem;
        font-size: 2rem;
        font-weight: 100;
        background-color: rgba(255, 255, 255, 0);
        color: white;
        border-style: solid;
        border-width: 2px;
        border-radius: 10px;
        padding: 3px;
        padding-right: 20px;
    }

    .cont {
        height: 50vh;
    }

    img {
        width: 100vw;
    }

    .title-btn {
        position: absolute;
        top:  50%;
        left: 10%;
        transform: translate(0, -50%);
    }

    h1 {
        color: white;
        font-size: 4rem;
        font-weight: 300;
    }
</style>