
<script>
 import '@fortawesome/fontawesome-free/css/all.min.css';
</script>

<footer id="footer", class="footer">
  <!-- svelte-ignore a11y-missing-attribute -->
  <div class="left"> <!-- Add this div -->
    <a class="copyright">© 2024 Richland High School Robotics All Rights Reserved.</a>
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
  text-align: left !important;
  color: white;
  background-color: #292929;
  text-decoration: none;
  padding-right: 30px;
  white-space: nowrap;
}  
.contact{
  text-decoration: none;
  background-color: #292929;
  color: white;
  margin-left: 20px;
  margin-right: 20px;
  font-size: 30px;
    transition: transform 0.2s ease-in-out;
}
.contact:hover{
  color: #f5f5f5;
    transform: scale(1.05);
}
.footer{
  padding-left: 15%;
  display: flex; /* Add this line */
  justify-content: space-between; /* Add this line */
  background-color: #292929;
  padding-top: 30px;
  padding-bottom: 30px;
}

.left, .right {
  display: flex;
  align-items: center;
  padding-right: 5%;
}

@media screen and (max-width: 1200px) {
.copyright{
  transform: translateY(30px);
}
.contact{
  text-align: left !important;
  transform: translateX(-1000px);
  margin-left: 30px;
}
}

</style>
