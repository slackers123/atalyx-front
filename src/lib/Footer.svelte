<div class="footer">
    <div class="logo">Atalyx Games</div>
    <div class="contact">
        <a href="mailto:contact@atalyx.games">contact@atalyx.games</a>
        <p class="location">Austria, Vienna</p>
        <p class="important">(No Kangoroos here...)</p>
    </div>
    <div class="socials-prompt">
        <p class="prompt">Follow us!</p>
        <div class="socials">
            <a href="https://instagram.com/atalyx.games"><img src="insta.svg" alt="Instagram"></a>
            <a href="https://youtube.com/"><img src="youtube.svg" alt="YouTube" style="padding-top: 0.3rem;"></a>
            <a href="mailto:contact@atalyx.games"><p>@</p></a>
        </div>
    </div>
</div>

<style>
    *  {
        background-color: rgb(29, 26, 38);
        color: white;
    }

    .socials {
        display: grid;
        grid-template-columns: 3rem 3rem 3rem;
        padding-left: 50%;
        transform: translate(-12.5%);
    }

    .socials * {
        height: 2rem;
        font-size: 1.5rem;
    }

    a {
        text-decoration: none;
    }

    .logo {
        padding-left: 10vw;
        padding-top: 2rem;
        font-size: 1.5rem;
        font-weight: 300;
    }

    .footer {
        width: 100vw;
        height: 6rem;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
    }

    .contact {
        padding-top: 0.5rem;
        text-align: center;
    }

    .contact > * {
        margin: 0.5rem;
        font-size: small;
    }

    a {
        font-weight: bold;
    }

    .prompt {
        font-size: 1.5rem;
        font-weight: 400;
    }

    .socials-prompt {
        text-align: center;
        padding-top: 1rem;
    }
</style>