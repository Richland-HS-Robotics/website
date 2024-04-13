<svelte:head>
    <title>RHS Robotics Homepage</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>


<style>
    .video {
               max-width: 100%;
               height: auto;
           }
           .logo {
            text-align: center;
            z-index: 300000;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
        .logo-image{
            width: 250px;
            height: auto;
        }
        .heading1{
            text-align: center;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%,150px);
            color: white;
        }
</style>
   
   
       <video autoplay muted loop id="video", class="video">
           <source src="seamless-robot.mp4" type="video/mp4">
       </video>
   <div class="logo">
    <img src="logo_gear.svg" alt="Logo", class="logo-image"> <!-- Add logo -->
    </div>
    <h1 class="heading1">Welcome to RHS Robotics</h1>
    <span class="home-hero-sub-heading bodyLarge"></span>