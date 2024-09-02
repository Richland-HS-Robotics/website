<svg id="grey" width="50vw" height="50vw">
  <circle cx="25vw" cy="25vw" r="25vw" fill="#4e5565" />
</svg>
<svg id="yellow" width="50vw" height="50vw">
  <circle cx="25vw" cy="25vw" r="25vw" fill="var(--green)" />
</svg>
<h1>Get in touch</h1>
<div id="container">
  <div class="card">
    <div class="heading-div">
      <span class="fa-regular fa-envelope icon" id="icons"></span>
      <span class="heading">Email us</span>
    </div>

    <span class="contact">
      <a href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
    </span>
  </div>
  <div class="card">
    <div class="heading-div">
      <span class="fa-brands fa-instagram icon" id="icons"></span>
      <span class="heading">Instagram</span>
    </div>

    <span class="contact">
      <a href="https://www.instagram.com/rhs_robotics24/">@rhs_robotics24</a>
    </span>
  </div>
  <div class="card">
    <div class="heading-div">
      <span class="fa-brands fa-github icon" id="icons"></span>
      <span class="heading">Github</span>
    </div>

    <span class="contact">
      <a href="https://github.com/Richland-HS-Robotics">Richland-HS-Robotics</a>
    </span>
  </div>
  <div class="card">
    <div class="heading-div">
      <span class="fa-solid fa-location-dot icon" id="icons"></span>
      <span class="heading">Address</span>
    </div>

    <span class="contact">
      <a href="https://goo.gl/maps/rfdSa5RVQFdTAzDY7">
        930 Long Ave #1070, Richland, WA 99352
      </a>
    </span>
  </div>
</div>

<p>
  Also check us out at FTCScout: <a href="https://ftcscout.org/teams/15010"
    >https://ftcscout.org/teams/15010</a
  >
</p>

<style>
  #grey {
    position: absolute;
    top: -25px;
    left: -15vw;
    z-index: 0;
    filter: blur(150px);
    opacity: 0.5;
  }
  #yellow {
    position: absolute;
    top: 55px;
    left: 65vw;
    z-index: 0;
    filter: blur(250px);
    opacity: 0.25;
  }
  p {
    padding-top: 50px;
    padding-bottom: 200px;
    position: relative;
    z-index: 2;
  }
  #icons {
    margin-left: 2.5vw;
  }
  .icon {
    color: var(--text-color);
    font-size: 40px;
    /* margin-top: 5%; */
  }
  .heading-div {
    margin-top: 2.5vw;
    display: flex;
    flex-direction: column;
  }
  h1 {
    padding-top: 80px;
    padding-bottom: 50px;
    z-index: 2;
    position: relative;
  }
  #container {
    display: flex;
    flex-direction: row;
    width: 90vw;
    background-color: var(--bg-color);
  }
  .card {
    width: calc(90vw / 4 - 2vw);
    transform: translateX(-1vw);
    margin-left: 1vw;
    margin-right: 1vw;
    height: auto;
    border-radius: 7px;
    border: 1px solid var(--yellow);
    background-color: var(--secondary-bg-color);
    box-shadow: 0 0 15px var(--secondary-bg-color);
  }
  .heading {
    font-size: 30px;
    /* margin-left: auto;
       margin-right: 25%; */
    display: block;
    color: var(--text-color);
    margin-left: 2.5vw;
    margin-top: 30px;
  }
  .contact {
    color: var(--text-color);
    font-size: 16px;
    width: 100%;
    display: block;
    margin-top: 5%;
    margin-left: 2.5vw;
    margin-bottom: 2.5vw;
    max-width: calc(90vw / 4 - 7vw);
  }
  @media screen and (max-width: 736px) {
    #container {
      flex-direction: column;
    }
    .card {
      width: 86vw;
      margin-bottom: 4vw;
      margin-top: 4vw;
    }
    .contact {
      margin-left: 5vw;
      max-width: 81vw;
      margin-bottom: 5vw;
    }
    #icons {
      margin-left: 5vw;
    }
    .heading {
      margin-left: 5vw;
    }
    p {
      padding-bottom: 25px;
    }
  }
</style>
