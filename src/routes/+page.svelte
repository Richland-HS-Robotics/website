<script>
  import Header from "$lib/Header.svelte";
  import Footer from "$lib/Footer.svelte";
  import CarouselSection from "$lib/CarouselSection.svelte";
  import Banner from "$lib/Banner.svelte";

  let count = 0;
</script>

<svelte:head>
  <title>RHS Robotics</title>
</svelte:head>

<Banner />

<div id="main">
  <p class="content">
    We are a robotics club from Richland High School in Richland, WA. We
    participate in the anual
    <a href="https://www.firstinspires.org/robotics/ftc">FIRST Tech Challenge</a
    >, where we build robots and compete against other teams.
  </p>

  <CarouselSection />

  <br />

  <h2>Contact Us</h2>

  <div id="contact">
    <p>
      Please feel free to contact us by email or Instagram message. You are also
      welcome to look at our code on Github.
    </p>
    <ul>
      <li>
        <i class="fa-solid fa-envelope" />
        <a href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
      </li>
      <li>
        <i class="fa-brands fa-instagram" />
        <a href="https://www.instagram.com/rhs_robotics.club/"
          >@rhs_robotics.club</a
        >
      </li>
      <li>
        <i class="fa-brands fa-github" />
        <a href="https://github.com/Richland-HS-Robotics"
          >Richland-HS-Robotics</a
        >
      </li>
      <li>
        <i class="fa-solid fa-location-dot" />
        <a href="https://goo.gl/maps/rfdSa5RVQFdTAzDY7"
          >930 Long Ave, Room 1070, Richland, WA 99352</a
        >
      </li>
    </ul>
  </div>

  <div id="aboutFirst">
    <img
      width="25%"
      src="FIRST_logos/FIRSTTech_iconHorz_RGB.png"
      alt="FIRST Centerstage logo"
    /> <br />
    <p class="content">
      Our club participates in the <em>FIRST</em> Tech Challenge, a competitions
      where teams of up to 15 members build a robot and compete with it.
    </p>

    <a class="button" href="https://www.firstinspires.org/robotics/ftc"
      >Learn More</a
    >

    <button>Learn More</button>
  </div>
</div>

<style>
  #main {
    width: 70%;
    margin: 0 auto;
    justify-content: center;
    text-align: center;
  }

  p.content {
    text-align: left;
    max-width: 38em;
    margin: 0 auto;
    margin-bottom: 2em;
    margin-top: 2em;
    /* padding-right: 10em; */
  }

  #contact {
    display: flex;
    justify-content: center;
    margin: 0 auto;
  }
  #contact ul {
    list-style: none;
    text-align: left;
    font-size: 1.3em;
  }
  #contact > ul > li > i {
    font-size: 1.5em;
    vertical-align: middle;
  }
  #contact p {
    text-align: left;
    max-width: 30em;
    margin-top: 3em;
  }

  a.button {
    appearance: button;
    text-decoration: none;
  }
</style>
