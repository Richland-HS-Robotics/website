<header id="header">
  <a id="logo" href="/">
    <img src="Logo_C_Dark.svg" />
    <span>RHS Robotics</span>
  </a>
  <nav class="navbar-container">
    <div id="menu">
      <ul class="links">
        <li><a href="about.html">About</a></li>
        <li><a href="robots.html">Robots</a></li>
        <li><a href="sponsors.html">Sponsors</a></li>
      </ul>
      <a href="#menu" class="close"></a>
    </div>
  </nav>

  <nav>
    <a href="#menu">Menu</a>
  </nav>
</header>

<!-- <style>
     #header {
   -moz-align-items: center;
   -webkit-align-items: center;
   -ms-align-items: center;
     align-items: center;
     display: -moz-flex;
     display: -webkit-flex;
     display: -ms-flex;
     display: flex;
   -moz-justify-content: space-between;
   -webkit-justify-content: space-between;
   -ms-justify-content: space-between;
     justify-content: space-between;
     background: #111111;
     color: rgba(255, 255, 255, 0.5);
     cursor: default;
     height: 3.25rem;
     left: 0;
     line-height: 3.25rem;
     position: fixed;
     top: 0;
     width: 100%;
     z-index: 10001; }

     #header > .logo {
     color: #ffffff;
     font-size: 1rem;
     font-weight: 600;
     height: inherit;
     line-height: inherit;
     padding: 0 1.25rem;
     text-decoration: none; }
     #header > nav > a {
     color: inherit;
     display: inline-block;
     padding: 0 0.75rem;
     text-decoration: none; }
     #header > nav > a:hover {
     color: #ffffff; }
     #header > nav > a[href="#menu"] {
     text-decoration: none;
   -webkit-tap-highlight-color: rgba(0, 0, 0, 0); }
     #header > nav > a[href="#menu"]:before {
   -moz-osx-font-smoothing: grayscale;
   -webkit-font-smoothing: antialiased;
     font-family: FontAwesome;
     font-style: normal;
     font-weight: normal;
     text-transform: none !important; }
     #header > nav > a[href="#menu"]:before {
     content: '\f0c9';
     margin: 0 0.5rem 0 0; }
     #header > nav > a + a[href="#menu"]:last-child {
     border-left: solid 1px rgba(255, 255, 255, 0.25);
     margin-left: 0.5rem;
     padding-left: 1.25rem; }
     #header > nav > a:last-child {
     padding-right: 1.25rem; }
     @media screen and (max-width: 736px) {
     #header > nav > a {
     padding: 0 0.5rem; }
     #header > nav > a + a[href="#menu"]:last-child {
     margin-left: 0.25rem;
     padding-left: 1rem; }
     #header > nav > a:last-child {
     padding-right: 1rem; } }
     @media screen and (min-width: 700px) {
     #header > nav > a[href="#menu"]{
     display: none;
     }


     #menu {
     position: static !important;
     visibility: visible !important;
     opacity: 1 !important;
     height: 100% !important;
     display: block !important;
     padding: 0 0 !important;
     transform: none !important;
     }


     .links{
     padding: 0 0 !important;
     box-shadow: none;
     display: flex;
     position: static;
     flex-direction: row;
     width: 100%;
     height: 100%;
     margin: 0 0 !important;
     overflow: hidden;
     }

     #menu > ul.links > li > a{
     border-top: none !important;
     margin-left: 1em;
     margin-right: 1em;
     }

     #menu > a.close {
     display: none;
     }
     }

     </style> -->

<style>
  @import url("https://fonts.googleapis.com/css?family=Raleway:200,300,400,500,600");

  header {
    font-family: "Raleway", Arial, Helvetica, sans-serif;
    align-items: center;
    display: flex;
    justify-content: space-between;
    background: #211c1e;
    color: #dddde3;
    position: sticky;
    height: 3.25rem;
    left: 0;
    top: 0;
    width: 100%;
    line-height: 3.25rem;
    z-index: 10001;
  }

  ul {
    display: flex;
    flex-direction: row;
    overflow: hidden;
    margin-bottom: 0;
  }

  li,
  a {
    color: #dddde3;
    /* Platinum Text color*/
    text-decoration: none;
    list-style-type: none;
    position: static;
    padding-left: 0;
    padding-right: 0;
  }

  li > a {
    margin-left: 1em;
    margin-right: 1em;
  }

  #logo {
    display: inline;
    color: #025d03;
    font-size: 2rem;
    font-weight: 600;
    height: inherit;
    line-height: 100%;
    padding: 0 1.25rem;
    text-decoration: none;
  }

  #logo img {
    vertical-align: middle;
    height: 100%;
  }

  #logo span {
    vertical-align: middle;
  }
</style>
