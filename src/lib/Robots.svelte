
<div class="image">
    <section id="about", class="about">
        <h1 class="header">Our Robots</h1>
    
        <p>
            RHS Robotics is a dynamic club that provides students with hands-on
            experience in designing, building, and programming robots for exciting
            competitions like the FIRST Tech Challenge. Our team fosters creativity,
            teamwork, and problem-solving skills in a fun and challenging
            environment. Join us to explore the world of robotics and unleash your
            potential! 
        </p>
        <!-- svelte-ignore a11y-missing-attribute -->
            <div class="image-container">
            <h2>The Robot Title</h2>
            <p>A sample description of the robot</p>
            <div class="image-padding">
            <img src="robot.jpg" alt="robot", class="image">
            </div>
            </div>


            <div class="image-container">
 <div class="image-padding">
            <img src="robot.jpg" alt="robot", class="image">
            </div>
            <h2>The Robot Title</h2>
            <p>A sample description of the robot</p>
           
            </div>

            <div class="image-container">
            <h2>The Robot Title</h2>
            <p>A sample description of the robot</p>
            <div class="image-padding">
            <img src="robot.jpg" alt="robot", class="image">
            </div>
            </div>
        <a href="/", class="button">VIEW ALL</a>
    </section>
    
        </div>
    
    
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
    
    .image{
        height: auto;
        width: 40em;
    }
    .image-padding{
        background-color: #c8c8c8;
        padding: 1em;
    }
    .image-container{
        width: 49em;
        columns: 2;
    }
    p{
        max-width: 50em;
        text-align: justify;
    }
    h2{
        color: black;
    }
        .about{
            margin-left: 33%;
            color: black;
        }
        .header{
            color: black;
            padding-top: 50px;
        }
        .image{
            background-image: url(gears_background.jpg);
            width: 100%;
            height: auto;
            background-attachment: fixed;
        }
        .button{
            text-decoration: none;
            color: white;
            background-color: var(--rhs-green);
            margin-top: 50px;
            padding-top: 5px;
            padding-bottom: 5px;
            font-weight: normal;
            border-radius: 0%;
            margin-bottom: 100px;
        }
        .button:hover{
            color: var(--white-hover);
            background-color: var(--rhs-green-hover);
        }
    </style>
