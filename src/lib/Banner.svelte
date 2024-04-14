<section>
  <video playsinline autoplay muted>
    <source src="animation.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <div class="content">
    <!-- <img src="Logo_C_Dark.svg" /> -->
    <svg viewbox="0 0 600 600" width="35%">
      <!-- <circle
           id="circularPath1"
           cx="300"
           cy="285"
           r="250"
           transform="rotate(190 300 300)"
           fill="transparent"
           />
           <circle
           id="circularPath2"
           cx="300"
           cy="285"
           r="250"
           transform="rotate(90 300 300)"
           fill="transparent"
           /> -->
      <image
        x="0"
        y="0"
        id="logo"
        href="Logo_C_Dark_WText.svg"
        width="600"
        height="600"
      />
      <!-- <text width="500" class="logoText">
           <textPath xlink:href="#circularPath1" id="logoTextText">
           Richland
           </textPath>
           </text>
           <text class="logoText">
           <textPath xlink:href="#circularPath2"> Robotics </textPath>
           </text> -->
    </svg>

    <!-- <h1>Richland Robotics</h1> -->
    <p>Some test paragraph content.</p>
  </div>
</section>

<style>
  section {
    background-color: #1f1f1f;
    /* color: rgba(255, 255, 255, 0.5); */
    color: #dbdbdb;
    align-items: center;
    display: flex;
    justify-content: center;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    border-top: 0;
    height: 45rem;
    min-height: 45rem;
    overflow: hidden;
    position: relative;
    text-align: center;
    width: 100%;
    text-align: center;
  }

  div {
    opacity: 1;
    position: relative;
    z-index: 3;
    margin: 0 auto;
    width: 75rem;
    max-width: calc(100% - 6rem);
    overflow: hidden;
    animation-name: fadein;
    animation-duration: 4s;
    animation-delay: 2s;
    animation-fill-mode: backwards;
  }
  @keyframes fadein {
    0% {
      opacity: 0;
    }

    100% {
      opacity: 1;
    }
  }

  /* section:after {
    background: linear-gradient(135deg, #008400 0%, #f7d600 74%);
    content: " ";
    display: block;
    height: 100%;
    left: 0;
    opacity: 0.6;
    position: absolute;
    top: 0;
    width: 100%;
    z-index: 1;
    }
  */
  section h1 {
    font-size: 4rem;
    margin-bottom: 1rem;
    /* color: #9590a8; */
    color: #dbdbdb;
    /*Cool Gray (text)*/
  }

  video {
    position: absolute;
    top: 0;
    /* left: 0; */

    object-fit: cover;
    /* width: 100%; */
    height: 100%;
    z-index: 0;
  }

  .content {
    z-index: 1;
  }

  .logoText {
    font-size: 5rem;
    /* fill: #025d03; */
    fill: #ffdd00;
    font-weight: bold;
  }
</style>
