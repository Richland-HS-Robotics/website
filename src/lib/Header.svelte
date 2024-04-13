<svelte:head>
    <title>RHS Robotics Homepage</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>

<script>
    let showMenu = false;
    function toggleMenu() {
        showMenu = !showMenu;
    }
</script>

<style>
:root{
    --rhs-green: #025D03;
    --rhs-green-hover: #013d02;
    --white-hover: #b1b1b1;
    --menu: #333;
    --menu-hover: #111;
    --robotics-grey: #808080;
    --transition-duration: 0.5s;
}
.navigation{
    background-color: var(--menu);
    display: flex;
    align-items: center;
    justify-content: space-between;
    transition: padding-left var(--transition-duration);
}
.nav-text{
    text-decoration: none;
    color: white;
    font-size: 15px;
    padding: 30px;
    display: inline-block;
    transition: opacity var(--transition-duration);
}
.logo-text{
    text-decoration: none;
    color: white;
    font-size: 15px;
    padding-left: 30px;
    display: inline-block;
}
.nav-text:hover{
    color: var(--white-hover);
    background-color: var(--menu-hover);
}
.button-donate{
    text-decoration: none;
    color: white;
    padding: 30px;
    background-color: var(--rhs-green);
    display: inline-block;
    transition: opacity var(--transition-duration);
}
.button-donate:hover{
    color: var(--white-hover);
    background-color: var(--rhs-green-hover);
}
.logo {
    height: 50px;
    vertical-align: middle;
}
.rhs {
    color: var(--rhs-green);
    font-size: 30px;
    text-decoration: none;
}
.robotics {
    color: var(--robotics-grey);
    font-size: 30px;
    text-decoration: none;
}
.logo-container {
    display: flex;
    align-items: left;
}
.burger-menu {
    display: none;
    cursor: pointer;
    color: white;
    font-size: large;
    padding-left: 30px;
    padding-right: 30px;
    transition: transform var(--transition-duration);
}
@media screen and (max-width: 1200px) {
    .nav-text, .button-donate {
        display: none;
        opacity: 0;
    }
    .burger-menu {
        display: block;
    }
    .show-menu {
        display: block;
        opacity: 1;
    }
    .navigation.show-menu {
        padding-left: 0;
    }
    .burger-menu.open {
        transform: rotate(90deg);
    }
    .navigation {
        flex-direction: column;
    }
    .logo-container {
        order: 1;
        text-align: left;
    }
    .burger-menu {
        order: 3;
    }
}
</style>

<header>
<div class="navigation {showMenu ? 'show-menu' : ''}">
    <div class="logo-container">
        <a class="logo-text" href="/">
            <img class="logo" src="logo_gear.svg" alt="Logo">
            <span class="rhs">RHS</span>
            <span class="robotics">ROBOTICS</span>
        </a>
    </div>
    <div>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="about.html">ABOUT</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="robots.html">ROBOTS</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="events.html">EVENTS</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="join-us.html">JOIN US</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="contact.html">CONTACT</a>
        <a class="button-donate {showMenu ? 'show-menu' : ''}" href="donate.html">♥ DONATE!</a>
        <div class="burger-menu {showMenu ? 'open' : ''}" on:click={toggleMenu}> <i class="fa-sharp fa-solid fa-bars"></i></div>
    </div>
</div>
</header>