<script>
    import { page } from "$app/stores";
</script>
<div class="header">
    <div class="logo">Atalyx Games</div>
    <nav>
        <a href="/home"  style="text-decoration: {$page.routeId == "home" ? "underline" : "none"};">Home</a>
        <a href="/games" style="text-decoration: {$page.routeId?.substr(0, 5) == "games" ? "underline" : "none"};">Games</a>
        <a href="/team"  style="text-decoration: {$page.routeId == "team" ? "underline" : "none"};">Team</a>
    </nav>
    <div class="other">
        <div class="socials">
            <a href="https://instagram.com/atalyx.games"><img src="insta.svg" alt="Instagram"></a>
            <a href="https://youtube.com/"><img src="youtube.svg" alt="YouTube" style="padding-top: 0.3rem;"></a>
            <a href="mailto:contact@atalyx.games"><p>@</p></a>
        </div>
        <div class="menu"> 
            <img src="menu.svg" alt="Menu">
        </div>
    </div>
</div>

<div class="padding"></div>

<style>
    *  {
        background-color: rgb(29, 26, 38);
        color: white;
        z-index: 5;
    }

    .socials {
        display: grid;
        grid-template-columns: 3rem 3rem 3rem;
        padding-left: 10vw;
    }

    .socials * {
        height: 2rem;
        font-size: 1.5rem;
    }

    .menu img {
        padding-top: 1.25rem;
        height: 2.5rem;
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
        text-decoration: none;
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
    }
</style>