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
    .div-r{
        display: flex;
        width: 60vw;
        justify-content: flex-end;
    }
    .div-l{
        display: flex;
        width: 40vw;
        text-align: left;
    }
    .burger-menu{
        cursor: pointer;
        font-size: 24px;
        color: var(--text-color);
        display: none;
    }
    @media only screen and (max-width: 768px) {
        .text{
            display: none;
        }
        .burger-menu{
            display: flex;
        }
    }
</style>
<link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">

<header>
    <div class="div-l">
        <img src="logo_dark.png" alt="logo" class="logo">
    </div>
    <div class="div-r">
        <a href="/" class="text">About us</a>
        <a href="/" class="text">Members</a>
        <a href="/" class="text">Robots</a>
        <a href="/" class="text">Join us</a>
    </div>
    <div class="burger-menu">
        &#9776;
    </div>
</header>