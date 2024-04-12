<svelte:head>
    <title>RHS Robotics Homepage</title>
</svelte:head>

<style>
:root{
    --rhs-green: #025D03;
}
.button-donate{
    text-align: center;
    text-decoration: none;
    color: white;
    background-color: var(--rhs-green);
    padding: 30px;
    font-size: 15px;
}
.button-donate:hover {
    color: #b1b1b1; /* Set the color for the link when hovered */
    text-decoration: none; /* Remove underline on hover */
    cursor: pointer; /* Add a pointer cursor on hover */
    background-color: #131313;
}
.navigation{
    padding: 30px !important;
    margin: 0%;
    background-color: #333;
    text-align: right;
}
.nav-logo{
    text-decoration: none;
    text-align: left;
    padding-top: 30px;
    padding-bottom: 30px;
    padding-left: 15px;
    padding-right: 15;
    transform: 50%,0%;
    color: white;
    font-size: 15px;
}
.nav-logo:hover{
    padding-left: 30px;
}

.nav-text{
    text-decoration: none;
    text-align: right;
    padding-top: 30px;
    padding-bottom: 30px;
    padding-left: 35px;
    padding-right: 35px;
    color: white;
    font-size: 15px;
}
.nav-text:hover {
    color: #b1b1b1; /* Set the color for the link when hovered */
    text-decoration: none; /* Remove underline on hover */
    cursor: pointer; /* Add a pointer cursor on hover */
    background-color: #131313;
}

</style>
<header>
<div class="navigation">
    <a class="nav-text" , href="about.html">ABOUT</a>
    <a class="nav-text" , href="gallery.html">GALLERY</a>
    <a class="nav-text" , href="my-process.html">MY PROCESS</a>
    <a class="nav-text" , href="contact.html">CONTACT</a>
    <a class="button-donate" , href="donate.html">&hearts; DONATE!</a>
</div>
</header>