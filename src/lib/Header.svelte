<svelte:head>
    <title>RHS Robotics Homepage</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>

<style>
:root{
    --rhs-green: #025D03;
    --rhs-green-hover: #013d02;
    --white-hover: #b1b1b1;
    --menu: #333;
    --menu-hover: #111;
}
.navigation{
    background-color: var(--menu);
    text-align: right;
}
.nav-text{
    text-decoration: none;
    color: white;
    font-size: 15px;
    padding: 30px;
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
    margin-right: 5%;
    background-color: var(--rhs-green);
    display: inline-block;
}
.button-donate:hover{
    color: var(--white-hover);
    background-color: var(--rhs-green-hover);
}
</style>
<header>
<div class="navigation">
    <a class="nav-text" href="about.html">ABOUT</a>
    <a class="nav-text" href="gallery.html">ROBOTS</a>
    <a class="nav-text" href="my-process.html">EVENTS</a>
    <a class="nav-text" href="contact.html">JOIN US</a>
    <a class="nav-text" href="contact.html">CONTACT</a>
    <a class="button-donate" href="donate.html">♥ DONATE!</a>
</div>
</header>
