
<script>
    import Bio from "$lib/Bio.svelte";
  </script>

    <div class="about-background">
<div class="header">
<span class="about-header">Contact </span>
<img src="logo_gear.svg" alt="RHS Gear" class="logo">
<span class="rhs">RHS</span>
<span class="robotics">ROBOTICS</span>
</div>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>








  
  <div id="main">

<span class="about-header">Contact</span>
<div class="contact">
<p style="margin-right: 1ch;">You can contact us through email at</p>
<a href="mailto:contact@rhs-robotics.com" style="margin-right: 1ch; color:grey;">contact@rhs-robotics.com</a>
<p>or with the button below</p>
</div>
<a href="mailto:contact@rhs-robotics.com" class="button">CONTACT US!</a>
  </div>
  <style>
    .contact{
      display: flex;
    }

    .button{
        text-decoration: none;
        color: white;
        background-color: var(--rhs-green);
        margin-top: 25px;
        padding-top: 5px;
        padding-bottom: 5px;
        font-weight: normal;
        border-radius: 0%;
        margin-bottom: 100px;
    transition: transform 0.2s ease-in-out;
        vertical-align: top;
}
.button:hover{
    transform: scale(1.03);
        color: var(--white-hover);
        background-color: var(--rhs-green-hover);
    }
    .form{
      width: 75%;
      text-align: left;
      border-radius: 0px;
      outline: none;
      background-color: #d9d9db;
    transition: transform 0.2s ease-in-out;
    }
    .form:hover{
      transform: scale(1.03);
      background-color: #cacacc;
      
    }
    #main {
      width: 70%;
      padding-left: 15%;
      justify-content: left;
      text-align: left;
      background-color: white;
      /* grid-template-rows: 1; */
    }
  .form-container{
    background-color: #f4f4f6;
    padding: 24px;
    margin-bottom: 50px;
  }
    .about-background{
        background-image: url(gears_background.jpg);
        padding-left: 15%;
        padding-top: 50px;
        background-attachment: fixed;
        padding-bottom: 45px;
    }
.logo {
    padding-left: 15px;
    height: 50px;
    vertical-align:top;
}

    .about-header{
        font-size: 30px;
        color: black;
        text-align: left;
        padding-top: 50px;
        padding-bottom: 150px;
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
.header{
    padding-bottom: 30px;
}
  </style>

