

<div id="container">

    <!-- <img src="%sveltekit.assets%/nathan-portrait.jpg"> -->
    <img src="nathan-portrait.jpg">
    <div>
        <div id="header" class="p">
            <h3>Nathan </h3>
            <div>
                <span>President</span>
                <span>CAD</span>
                <span>Design</span>
            </div>
        </div>
        <p class="p">
            I love robotics. In middle school, I joined FLL and I continued in the
            First program with FTC once I reached high school. Through my time in
            robotics, I’ve developed many skills. I’ve learned to more effectively
            communicate and cooperate with teammates, utilizing all their different
            skills and talents. I’ve learned how to compete and excel during
            competitions while respecting and even helping opponents. I’ve gained
            mechanical abilities. Designing and building many robots over the years
            has helped me understand critical components to make designs proficient.
            I have also learned to use new tools like CAD to design custom parts and
            3D printers to fabricate the parts. Robotics has helped me gain many
            valuable skills and I’ve loved all the opportunities it has provided me.
        </p>
    </div>
</div>



<style>
 #container{
     width: 100%;
     display: flex;
     align-items: center;
     justify-content: space-between;
     padding: 1.5em;
     border-radius: 1.5em 1.5em;

     background-color: #ffff4d;

     /* border: solid 2px black; */
     box-shadow: 10px 10px grey;
 }

 #header{
     display: flex;
     justify-content: space-between;
     align-items: center;
 }

 img{
     height: auto;
     max-width: 25%;
     display: flex;
     margin-right: 3em;
     border-radius: 0.7em 0.7em;
 }

 .p{
     width: 70%;
 }

 p{
     text-align: justify;
 }

 span{
     font-size: 1.3em;
     background-color: #4d79ff;
     padding: 0.2em;
     border-radius: 0.4em 0.4em;
     margin-left: 0.1em;
     margin-right: 0.1em;
 }
</style>
