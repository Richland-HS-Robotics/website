<style>
    header{
        padding-top: 15px;
        padding-bottom: 15px;
        background-color: rgba(255,255,255,0);
        z-index: 1;
        display: flex;
        position: relative;
        margin-left: 5vw;
        margin-right: 5vw;
        justify-content: space-between;
        overflow: hidden;
    }
    .logo{
        width: 40px;
        height: 40px;
        text-align: left;
    }
    .text{
        color: var(--text-color);
        text-decoration: none;
        font-size: 20px;
        margin-left: 10px;
        margin-right: 10px;
        transition: all ease-in 0.1s;
        font-family: 'Open Sans', sans-serif;
    }
    .text:hover{
        color: var(--text-color-hover);
    }
    .div-links{
        display: flex;
        width: 60vw;
        justify-content: flex-end;
    }
    .burger-menu{
        cursor: pointer;
        font-size: 24px;
        color: var(--text-color);
        display: none;
        padding-left: 0;
        /* margin-left: 5vw; */
    }
    .burger-menu:hover{
        color: var(--text-color-hover);
    }
    .burger-menu #sidebar-menu{
        visibility: hidden;
        text-rendering: geometricPrecision;
        position: fixed;
        top: 0;
        left: -40%;
        width: /* 10em */ 40%;
        /* background: red; */
        height: 100%;
        transition: 0.3s;
    }
    @media only screen and (max-width: 768px) {
        .div-links{
            display: none;
        }
        .burger-menu{
            display: flex;
        }
    }
    #burger-input{
        display: none !important;
    }

    #burger-input:checked + .burger-menu #sidebar-menu{
        visibility: visible;
        left: 0;
    }
    #burger-input:checked ~ .overlay{
        visibility: visible;
        opacity: 0.6;
    }
    .burger-menu::before{
        display:none;
    }
    .overlay{
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        opacity: 0;
        visibility: hidden;
        transition: opacity .35s, visibility .35s, height .35s;
        overflow: hidden;
        background: black;
        z-index: -1;
    }

    #sidebar-menu ul li{
        color: var(--text-color);
        list-style-type: none;
        margin: 0;
        padding: 0;
    }

    #sidebar-menu ul{
        padding: 0;
        margin-left: 5vw;
        margin-top: 2em;
    }
</style>
<link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">

<header>
    <input type="checkbox" id="burger-input" class="burger-shower">
    <label class="burger-menu" for="burger-input">
    &#9776;
        <nav id="sidebar-menu">
            <ul>
                <li>Home</li>
                <li>Members</li>
                <li>Robots</li>
                <li>Join us</li>
            </ul>
        </nav>
    </label>


    <div class="div-logo">
        <img src="logo_dark.png" alt="logo" class="logo">
    </div>
    <div class="div-links">
        <a href="/" class="text">About us</a>
        <a href="/" class="text">Members</a>
        <a href="/" class="text">Robots</a>
        <a href="/" class="text">Join us</a>
    </div>

    <div class="overlay"></div>
</header>
