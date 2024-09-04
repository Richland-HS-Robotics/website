<script>
  let menuOpen = false;

  let menuButtons;
  let burgerInput;

  function toggleMenu() {
    menuOpen = !menuOpen;
  }

  function closeMenu() {
    menuOpen = false;
    burgerInput.checked = false; // Add this line to uncheck the checkbox
  }

  import { onMount } from 'svelte';

  onMount(() => {
    menuButtons = document.querySelectorAll("#sidebar-menu ul li a");
    burgerInput = document.getElementById("burger-input");

    menuButtons.forEach((button) => {
      button.addEventListener("click", () => {
        burgerInput.checked = false;
      });
    });

    // Add event listener to window scroll event
    window.addEventListener('scroll', () => closeMenu()); // Pass the closeMenu function as a reference
  });
</script>
<link
    href="https://fonts.googleapis.com/css?family=Open+Sans"
    rel="stylesheet"
/>

<header>
    <input type="checkbox" id="burger-input" class="burger-shower" />
    <label class="burger-menu" for="burger-input">
        &#9776;
        <nav id="sidebar-menu">
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/about">About Us</a></li>
                <li><a href="/robots">Robots</a></li>
                <li><a href="/contact">Contact</a> us</li>
                <li><a href="/involved">Get</a> involved</li>
            </ul>
        </nav>
    </label>

    <a href="/" class="div-logo">
        <img
            src="logos/Logo_C_Dark.svg"
            alt="logo"
            class="logo"
            id="logo-small"
        />
        <img
            src="logos/Logo_C_Dark_Horiz.svg"
            alt="logo"
            class="logo"
            id="logo-big"
        />
    </a>
    <div class="div-links">
        <a href="/about" class="text">About Us</a>
        <a href="/robots" class="text">Robots</a>
        <a href="/contact" class="text">Contact</a>
        <a href="/involved" class="text">Get involved</a>
    </div>

    <div class="overlay"></div>
</header>

<style>
    header {
        padding-top: 15px;
        padding-bottom: 15px;
        z-index: 10;
        display: flex;
        position: relative;
        padding-left: 5vw;
        padding-right: 5vw;
        justify-content: space-between;
        overflow: hidden;
    }
    .logo {
        /* width: 40px; */
        height: 40px;
        text-align: left;
    }
    .text {
        color: var(--text-color);
        text-decoration: none;
        font-size: 20px;
        margin-left: 10px;
        margin-right: 10px;
        transition: all ease-in 0.1s;
        font-family: "Open Sans", sans-serif;
    }
    .text:hover {
        color: var(--text-color-hover);
        cursor: pointer;
    }
    .div-links {
        display: flex;
        width: 60vw;
        justify-content: flex-end;
        z-index: 3;
    }
    .burger-menu {
        cursor: pointer;
        font-size: 24px;
        color: var(--text-color);
        display: none;
        padding-left: 0;
        /* margin-left: 5vw; */
    }
    .burger-menu:hover {
        color: var(--text-color-hover);
    }
    .burger-menu #sidebar-menu {
        visibility: hidden;
        text-rendering: geometricPrecision;
        position: fixed;
        top: 0;
        left: -95vw;
        width: /* 10em */ 40%;
        /* background: red; */
        height: 100%;
        transition: 0.3s;
    }
    @media only screen and (max-width: 768px) {
        .div-links {
            display: none;
        }
        .burger-menu {
            display: flex;
        }
    }
    #burger-input {
        display: none !important;
    }

    #burger-input:checked + .burger-menu #sidebar-menu {
        visibility: visible;
        left: 0;
    }
    #burger-input:checked ~ .overlay {
        visibility: visible;
        opacity: 0.6;
    }
    .burger-menu::before {
        display: none;
    }
    .overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        opacity: 0;
        visibility: hidden;
        transition:
            opacity 0.35s,
            visibility 0.35s,
            height 0.35s;
        overflow: hidden;
        background: black;
        z-index: -1;
    }

    #sidebar-menu ul li {
        color: var(--text-color);
        list-style-type: none;
        margin: 0;
        padding-top: 25px;
        font-size: 40px;
        width: 95vw;
    }

    #sidebar-menu ul {
        padding: 0;
        padding-left: 5vw;
        margin-top: 70px;
        background-color: var(--bg-color);
        width: 95vw;
        height: 100vh;
    }

    #logo-small {
        display: none;
    }

    @media only screen and (max-width: 768px) {
        #logo-small {
            display: inline;
        }

        #logo-big {
            display: none;
        }
    }
</style>
