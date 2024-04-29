<script>
    let showMenu = false;
    function toggleMenu() {
        showMenu = !showMenu;
    }
</script>

<style>
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
    vertical-align:top;
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
    padding-left: var(--left-margin);
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
            <img class="logo" src="logo_dark.png" alt="Logo">
            <span class="rhs">RHS</span>
            <span class="robotics">ROBOTICS</span>
        </a>
    </div>
    <div>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="/about">ABOUT</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="/">ROBOTS</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="/">EVENTS</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="/">JOIN US</a>
        <a class="nav-text {showMenu ? 'show-menu' : ''}" href="/contact">CONTACT</a>
        <a class="button-donate {showMenu ? 'show-menu' : ''}" href="/">♥ DONATE!</a>
        <button class="burger-menu {showMenu ? 'open' : ''}" on:click={toggleMenu} > <i class="fa-sharp fa-solid fa-bars"></i></button>
    </div>
</div>
</header>
