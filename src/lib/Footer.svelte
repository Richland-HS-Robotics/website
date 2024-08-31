
<script>
 import '@fortawesome/fontawesome-free/css/all.min.css';
</script>

<link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
<footer id="footer", class="footer">
  <!-- svelte-ignore a11y-missing-attribute -->
  <div class="left"> <!-- Add this div -->
    <p class="copyright">© 2024 Richland Robotics All Rights Reserved.</p>
  </div> <!-- Close the div -->
  <div class="right"> <!-- Add this div -->
    <a href="mailto:contact@rhs-robotics.com", class="contact"><i class="fa-regular fa-envelope"></i></a>
    <a href="https://www.instagram.com/richlandrobotics/", class="contact"><i class="fa-brands fa-instagram"></i></a>
    <a href="https://github.com/Richland-HS-Robotics", class="contact"><i class="fa-brands fa-github"></i></a>
    <a href="https://goo.gl/maps/rfdSa5RVQFdTAzDY7", class="contact"><i class="fa-solid fa-location-dot"></i></a>
  </div> <!-- Close the div -->
</footer>





<style>
  .copyright{
  color: var(--text-color);
  background-color: var(--bg-color);
  text-decoration: none;
    /* padding-right: 30px; */
    /* white-space: nowrap; */
  font-family: 'Open Sans', sans-serif;
  font-size: 20px;
}  
.contact{
  text-decoration: none;
  background-color: var(--bg-color);
  color: var(--text-color);
  margin-left: 1em;
  margin-right: 1em;
  font-size: 25px;
    transition: transform 0.2s ease-in-out;
}
.right a:last-child{
  margin-right: 0;
 }
.contact:hover{
  color: var(--text-color-hover);
}
#footer{
  display: flex; /* Add this line */
  background-color: var(--bg-color);
  padding-top: 30px;
  padding-bottom: 30px;
}

.left {
  display: flex;
  width: 70%;
  margin-left: 5vw;
}
.right{
  text-align: right;
  display: flex;
  margin-left: auto;
  margin-right: 5vw;
 }

@media screen and (max-width: 768px) {
  .left{
    width: 95%;
  }
  .right{
    width: 95%;
    text-align: left;
    padding-top: 15px;
    margin-left: 3vw;
  }
  #footer{
    flex-direction: column;
  }
}

 /* @media screen and (max-width: 1200px) {
    .copyright{
    transform: translateY(30px);
    }
    .contact{
    text-align: left !important;
    transform: translateX(-1000px);
    margin-left: 30px;
    }
    }
  */
</style>
