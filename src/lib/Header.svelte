<script>
    import { page } from "$app/stores";
</script>
<div class="header">
    <div class="logo">Atalyx Games</div>
    <nav>
        <a href="/home"  style="text-decoration: {$page.routeId == "home" ? "underline" : "none"};">Home</a>
        <a href="/games" style="text-decoration: {$page.routeId == "games" ? "underline" : "none"};">Games</a>
        <a href="/team"  style="text-decoration: {$page.routeId == "team" ? "underline" : "none"};">Team</a>
    </nav>
    <div class="other">
        <div class="socials">
            Insta YT Email
        </div>
        <div class="menu"> Menu</div>
    </div>
</div>

<div class="padding"></div>

<style>
    *  {
        background-color: rgb(29, 26, 38);
        color: white;
    }

    nav {
        display: flex;
        justify-content: space-between;
    }

    .logo {
        padding-left: 5vw;
        padding-top: 1.5rem;
        font-size: 1.5rem;
        font-weight: 300;
    }
    a {
        padding-top: 1.5rem;
        font-weight: bold;
        font-size: 1.2rem;
    }

    .header {
        position: fixed;
        width: 100vw;
        height: 5rem;
        display: grid;
        grid-template-columns: 40vw 20vw 40vw;
    }
    .padding {
        width: 100vh;
        height: 5rem;
    }

    .other {
        display: flex;
        justify-content: space-around;
        padding-top: 1.5rem;
    }
</style>