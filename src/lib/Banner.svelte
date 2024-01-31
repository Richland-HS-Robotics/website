

<section>
    <div>
        <h1>Richland High School Robotics</h1>
        <p>Some test paragraph content.</p>
    </div>
</section>





<style>
 section{
     background-color: #111111;
     color: rgba(255,255,255,0.5);
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
 }

 div{
     transform: scale(1.0);
     transition: opacity 1s ease, transform 1s ease;
     opacity: 1;
     position: relative;
     z-index: 3;
     margin: 0 auto;
     width: 75rem;
     max-width: calc(100% - 6rem);
 }

 section:after{
     background: linear-gradient(135deg, #008400 0%, #f7d600 74%);
     content: ' ';
     display: block;
     height: 100%;
     left: 0;
     opacity: 0.6;
     position: absolute;
     top: 0;
     width: 100%;
     z-index: 1;
 }


 section h1{
     font-size: 4rem;
     margin-bottom: 1rem;
     color: #9590A8;
     /*Cool Gray (text)*/
 }
</style>
