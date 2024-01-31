
<script>
 import Bio from "$lib/Bio.svelte";
</script>


<h1>Members</h1>



<div id="main">

    <Bio name="Nathan"
         roles={["President", "CAD", "Design"]}
         src="nathan-portrait.jpg"
    >
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

    </Bio>

    <br/>

    <Bio name="Ian"
         roles={["Build","Repair"]}
         src="ian-portrait.jpg"
         reversed
    >
        I enjoy sports such as basketball, soccer and football. I enjoy hunting,
        fishing, and being outdoors. I joined robotics my freshman year and have been
        doing robotics for 7 years participating on FLL teams. I have always enjoyed
        building things out of legos and erector sets. I mostly do building and repair
        on the robot and help out where else I am needed.
    </Bio>
</div>


<style>


 #main{
     width:70%;
     margin: 0 auto;
     justify-content: center;
 }
</style>
