
<script>
    import Bio from "$lib/Bio.svelte";
  </script>

    <div class="about-background">
<div class="header">
<span class="about-header">About </span>
<img src="logo_gear.svg" alt="RHS Gear" class="logo">
<span class="rhs">RHS</span>
<span class="robotics">ROBOTICS</span>
</div>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>








  
  <div id="main">

<span class="about-header">Members</span>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    <div class="grid">
      <Bio
        name="Nathan"
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
        has helped me understand critical components to make designs proficient. I
        have also learned to use new tools like CAD to design custom parts and 3D
        printers to fabricate the parts. Robotics has helped me gain many valuable
        skills and I’ve loved all the opportunities it has provided me.
      </Bio>
  
      <Bio
        name="Sahir"
        roles={["VP", "Outreach", "Portfolio"]}
        src="sahir-portrait.jpg"
      >
        Robotics has been a large part of my life since the 5th grade, when I
        joined a local FLL team. Through our excellent teamwork and creativity, we
        made it to state each year I participated. After I aged out of FLL, I
        wanted to continue to explore this interest, so I joined FTC Robotics
        through my school and have never looked back. My specialties on the team
        include planning and leadership---one of the main reasons I'm captain---as
        well as coding. I have gotten a taste of every part of robotics throughout
        my journey and always jump to help out those in my team, the FTC team we
        mentor, and local FLL teams, planning and leading the FLL Preview
      </Bio>
  
      <Bio
        name="Calvin"
        roles={["Coding", "Electronics"]}
        src="calvin-portrait.jpg"
      >
        Since I took a Lego Robotics class in elementary school, I have been
        interested in programming computers; I have been programming ever since.
        When I came across the RHS robotics club, I joined it and have enjoyed it.
        My primary specialty on the team is programming, so I am the main
        programmer on the team. Programming a robot poses unique challenges
        compared to programming more traditional applications (you need the robot
        to test your code, and you have to be careful not to break it), and it has
        been interesting to learn this kind of programming.
      </Bio>
  
      <Bio
        name="Tyler B"
        roles={["Co&#8209;Captain", "Outreach", "Drive", "Portfolio"]}
        src="tyler-portrait.jpg"
      >
        When I got to high school, my friend who had been in high school robotics
        told me to join. I decided to join, and I’ve had a lot of fun for the past
        3 years since being a part of Richland High’s FTC teams. This year, I have
        been focusing on mentoring the younger richland team, managing outreach,
        organizing fundraisers, as well as driving the robot at competitions. A
        very important part of what I've done this year is helping the two new
        Carmichael teams.
      </Bio>
  
      <Bio
        name="Fintin"
        roles={["Co&#8209;Captain", "Outreach", "Drive", "Portfolio"]}
        src="fintin-portrait.jpg"
      >
        I’ve always had a strong interest in computer science and engineering so
        when I saw robotics at the club fair in 9th grade I joined it. Since then
        I have learned lots about programming and design and have built lots of
        skills that will help me in my future career. Robotics helped me build my
        skill and develop new friendships. I have been a driver and a team captain
      </Bio>
  
      <Bio
        name="Emmett"
        roles={["Design", "CAD", "3D Printing"]}
        src="emmett-portrait.jpg"
      >
        I've been a part of an underwater robotics team for over 4 years now and
        always am looking for opportunities to do more engineering. I have had a
        lot of fun doing FTC, an engineering challenge with a completely different
        set of challenges from what I am used to from my underwater robotics
        experiences. I've learned a lot of skills in the areas of designing and
        building, and this year in particular I have greatly improved my CAD
        skills.
      </Bio>
  
      <Bio name="Ian" roles={["Build", "Repair"]} src="ian-portrait.jpg">
        I enjoy sports such as basketball, soccer and football. I enjoy hunting,
        fishing, and being outdoors. I joined robotics my freshman year and have
        been doing robotics for 7 years participating on FLL teams. I have always
        enjoyed building things out of legos and erector sets. I mostly do
        building and repair on the robot and help out where else I am needed.
      </Bio>
  
      <Bio
        name="Benjamin"
        roles={["Design", "Build"]}
        src="benjamin-portrait.png"
      >
        I enjoy learning about math and science, so when robotics was strongly
        recommended in my Junior year, I decided to join. Over the last year, I
        learned the skills, designing, and testing that I implemented this year
        when designing, testing, and implementing the drone into our design. I
        have enjoyed the community our club has created, supporting each other as
        we have strived together to create the best robot possible.
      </Bio>
  
      <Bio name="Tyler H" roles={["Design", "Build"]} src="tylerh-portrait.jpg">
        No text...
      </Bio>
    </div>
  </div>
  
  <style>
    #main {
      width: 70%;
      padding-left: 15%;
      justify-content: left;
      text-align: left;
      background-color: white;
      /* grid-template-rows: 1; */
    }
  
    .grid {
      margin-top: 4em;
      display: grid;
      grid-template-columns: auto auto;
      gap: 3em;
      background-color: white;
      padding-bottom: 100px;
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
 p{
        max-width: 50em;
        text-align: justify;
    }
    .about-header{
        font-size: 30px;
        color: black;
        text-align: left;
        padding-top: 50px;
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

