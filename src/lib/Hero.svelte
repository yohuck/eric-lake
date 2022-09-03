<script>
    // import pic from '../assets/eric.png'
</script>

<section>
    <div class="grp">
        <h1 class="welcome-hero">
          Howdy, friend.<span class="second"> <br> I'm Eric</span>.
        </h1>
        <p class="welcome-text">I'm a front-end developer who loves building <span class="ayo">bold</span> UI. 
           I spent the first decade of my career building <span class="ayo">customer processes</span> and have become an expert in the people on the other side of the screen.
           I spent the last <span class="ayo">9 months</span> learning to build the web. </p>
        
           <button class="primary">View my resume.</button>
    </div>

    <div class="circle-3">

    </div>
    <div class="photo">
        <div class="circle"></div>
        <div class="circle"></div>
        <div class="circle"></div>
    </div>
   



</section>



<style>
@import "open-props/style";
@import "open-props/normalize";
@import "open-props/masks/edges";

.grp{
    width: 100%;
}


    h1{
 
         color: var(--teal-5);
         line-height: var(--font-lineheight-1);
  font-size: var(--font-size-8);
  font-weight: var(--font-weight-9);
  font-family: var(--font-sans);
  margin-bottom: 0;
  text-shadow: 2px 3px 1px var(--blue-2);
    }

    .welcome-text{
        position: relative;
        color: var(--red-0);
        word-wrap: break-word;
        line-height: var(--font-lineheight-2);
        font-size: var(--font-size-2);
        font-weight: var(--font-weight-3);
    }



    .photo{
        width: 70%;

        margin-right: var(--size-10);
        aspect-ratio: 1;
        animation: grad 7s linear 0s infinite alternate none;
        position: relative;

        background-position-x:0px;
        background-image: var(--gradient-2);
        background-size: 2000px 2000px;

        border-radius: 999px;
        z-index: 7;
        opacity: 1;
    }

    .circle{
        width: 140%;
        aspect-ratio: 10;
        transform-origin: center;
        transform: translateX(-15%)translateY(200%) rotate(10deg);
        border-top: 3px dashed var(--yellow-4);
        border-left: 1px dashed var(--blue-4);
        border-right: 1px dashed var(--blue-6);
        border-radius: 50%;
        z-index: 2;
        mask-clip:  unset;
        animation: round 5s linear 0s infinite running none;
        /* background-color: var(--grape-9); */
        opacity: 1;
    }

    .circle:nth-of-type(odd){
        border-top: 8px dotted var(--blue-2);
        border-left: 3px dashed var(--yellow-4);
        border-right: 8px dotted var(--blue-6);
        animation: roundy 30s linear 0s infinite running none;
        transform: translateX(-15%)translateY(150%) rotate(10deg);
    }
    .circle:nth-of-type(1){
        border-top: 5px dotted var(--blue-2);
        border-left: 5px dotted var(--blue-4);
        border-right: 5px dotted var(--blue-6);
        animation: roundy 7s linear 0s infinite running none;

        transform: translateX(-15%)translateY(320%) rotate(10deg);

    }

    /* .circle-4{
        transform: translateY(30%) rotate(10deg);
        border-radius: 999px;
        border-top: 5px dotted var(--red-5);
        border-left: 5px dotted var(--red-5);
        border-right: 5px dotted var(--red-5);
        position: absolute;
        aspect-ratio: 6;
        width: 120%;
    } */



    /* .second{
        color: var(--red-9);
        text-shadow: none;
    } */

    .ayo{
        /* background-color: var(--gray-9); */
        color: var(--teal-5);
        font-weight: var(--font-weight-9);
    }

    section{
        /* max-width: 900px; */
        height: 100vh;
        margin: 0 auto;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;

        padding: var(--size-10);
        background-color: var(--cyan-0);
        line-height: var(--font-lineheight-0);
        /* -webkit-mask: var(--mask-edge-drip-bottom); */
   
  background-image: var(--gradient-16);


    }

    button {
  background: white;
  color: var(--indigo-8);
  font-size: var(--font-size-3);
  padding-inline: var(--size-8);
  padding-block: var(--size-3);
  border-radius: var(--radius-2);
  box-shadow: var(--shadow-2);
  margin-top: var(--size-5);
}

button.primary {
  background: var(--teal-5);
  font-weight: var(--font-weight-7);
  text-shadow: 0 1px 0 var(--red-2);
  color: white;
}

button.primary:hover {
  background: var(--teal-4);
  color: var(--indigo-7);
  text-shadow: none;
}


@keyframes grad{
    0% {
        background-position: -1200px -1200px;
    }
    22% {
    }
    47% {
        background-position: 0px 0px;
        transform:  rotate(2deg);
    }
    76% {
    }
    100% {
        background-position: -100px -00px;
    }
}

@keyframes round{
    0% {
        border-top: 8px dotted var(--blue-4);
        border-left: 8px dotted var(--blue-6);
        border-right: 8px dotted var(--blue-8);
    }
    22% {
    }
    47% {

    }
    76% {
    }
    100% {

    }
}

@keyframes roundy{
    0% {
        border-top: 4px dashed var(--blue-3);
        border-left: 4px dashed var(--blue-6);
        border-right: 4px dashed var(--blue-8);
    }
    22% {
    }
    47% {

    }
    76% {
        border-top: 4px dashed var(--blue-5);
        border-left: 4px dashed var(--blue-6);
        border-right: 4px dotted var(--blue-8);
    }
    100% {

    }
}

</style>