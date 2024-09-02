<h1>Get in touch</h1>
<div id="container">
  <div class="card">
    <div class="heading-div">
      <span class="fa-regular fa-envelope icon"></span>
      <span class="heading">Email us</span>
    </div>

      <span class="contact">
        <a href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
      </span>
  </div>
  <div class="card">

    <div class="heading-div">
      <span class="fa-brands fa-instagram icon"></span>
      <span class="heading">Instagram</span>
    </div>

    <span class="contact">
      <a href="https://www.instagram.com/rhs_robotics24/">@rhs_robotics24</a>
    </span>

  </div>
  <div class="card">
    <div class="heading-div">
      <span class="fa-brands fa-github icon"></span>
      <span class="heading">Github</span>
    </div>

    <span class="contact">
      <a href="https://github.com/Richland-HS-Robotics">Richland-HS-Robotics</a>
    </span>

  </div>
  <div class="card">
    <div class="heading-div">
      <span class="fa-solid fa-location-dot icon"></span>
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
  .icon{
    color: var(--text-color);
    font-size: 40px;
    margin-left: 5%;
    /* margin-top: 5%; */
  }
 .heading-div{
   margin-top: 5%;
   display: flex;
 }
  h1 {
    padding-top: 80px;
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
    height: 200px;
    border-radius: 7px;
    border: 1px solid var(--yellow);
    background-color: var(--secondary-bg-color);
    box-shadow: 0 0 15px var(--secondary-bg-color);
  }
  .heading{
    font-size: 30px;
    /* margin-left: auto;
       margin-right: 25%; */
    display: block;
    margin: 0 auto;

    color: var(--text-color);
  }
  .contact{
    color: var(--text-color);
    font-size: 24px;
    text-align: center;
    width: 100%;
    display: block;
    margin-top: 5%;
    /* margin-left: 10%; */
  }
  @media screen and (max-width: 736px) {
    #container{
      flex-direction: column;
    }
    .card{
      width: 86vw;
      margin-bottom: 4vw;
      margin-top: 4vw;
    }
  }
</style>
