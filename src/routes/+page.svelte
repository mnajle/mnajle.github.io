<div class="content">
    <div class="left-side">
        <div class="header">
            <div class="name">Maximiliano Najle</div>
            <div class="greet">
                Software Developer<br />from <span class="arg">Argentina</span>
            </div>
            https://chaseohlson.com/ https://bepatrickdavid.com/
        </div>
        <div class="links">
            <div class="link">
                <a href="mailto:maximilianonajle@gmail.com/" target="_blank">
                    <img class="icon" src="mail.svg" /><span
                        >maximilianonajle@gmail.com</span
                    >
                </a>
            </div>
            <div class="link">
                <a href="https://www.linkedin.com/in/mnajle/" target="_blank">
                    <img class="icon" src="linkedin.svg" />
                    <span>/mnajle</span>
                </a>
            </div>
            <div class="link">
                <a href="/cv.pdf" download="cv.pdf">
                    <img class="icon" src="download-file.svg" /><span
                        >cv.pdf</span
                    >
                </a>
            </div>
        </div>
    </div>
    <div class="right-side">
        <div></div>
        <!-- <p></p> -->
    </div>
</div>

<style>
    :root {
        --blue: #052f5f;
        --white: #fff6f6;
        --black: #090909;
        --bluel: #005377;
        --red: #d72638;
    }

    .icon {
        width: 24px;
        padding: 8px;
        background: var(--white);
        border-radius: 15%;
    }
    /*
    body {
        background-color: #090909;
        font-family: "Open Sans", sans-serif;
        font-optical-sizing: auto;
        font-style: normal;
        font-variation-settings: "wdth" 100;
    }*/

    .content {
        max-height: 98vh;
        height: 98vh;
        overflow-y: hidden;
        display: grid;
        color: var(--white);
    }

    .left-side {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        padding: 8px;
    }

    .left-side .header {
        font-size: 25px;
        display: flex;
        flex-direction: column;
        width: fit-content;
    }

    .name {
        font-size: 4rem;
    }

    .links {
        display: flex;
        flex-direction: column;
    }

    .links a {
        display: flex;
        align-items: center;
        color: var(--white);
        text-decoration: none;
        font-size: 20px;
    }

    .arg {
        color: #4fc3f7;
    }

    .links > .link > a > img {
        margin-right: 8px;
    }

    .links > .link {
        margin-bottom: 4px;
    }

    @media (min-width: 640px) and (max-width: 1024px) {
        .content {
            grid-template-columns: 1fr;
            margin: 32px;
        }
        .left-side {
            grid-row: 2;
        }
        .right-side {
            grid-row: 1;
            width: 100%;
            display: flex;
            justify-content: end;
        }
        .links {
            justify-content: space-around;
        }
        .links i {
            font-size: 72px;
        }
    }

    @media (min-width: 1024px) {
        .content {
            grid-template-columns: 1fr 2fr;
        }
        .left-side {
            grid-column: 1;
        }
        .right-side {
            grid-column: 2;
        }
    }
    @media (min-width: 1590px) {
        .content {
            /* margin: 0 32px; */
        }
    }
</style>
