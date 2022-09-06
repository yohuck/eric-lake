<script>
    let ui = '';
    let uiChoices = ['b','bo','bol','bold', 'bold','bold', 'bold', 'i', 'in', 'inv', 'invi', 'invit', 'inviti', 'invitin', 'inviting', 'inviting', 'inviting', 'inviting', 'a', 'ac','acc','acce','acces','access','accessi','accessib','accessibl','accessible', 'accessible','accessible', 'accessible','w','wh','whi','whim','whims','whimsi','whimsic','whimsica','whimsical', 'whimsical','whimsical', 'whimsical','e','ef','eff','effe','effec','effect','effecti','effectiv','effective', 'effective','effective', 'effective']
    let customer = '';
    let customerChoices = ['c','cu','cus','cust','custo','custom','custome','customer','customer','customer','customer','customer','customer', 'u', 'us','use','user','user','user','user','user','c','cl','cli','clie','clien','client','client','client','client','client', 'p', 'pa', 'par', 'part', 'partn', 'partne', 'partner', 'partner', 'partner', 'partner', 'partner', 'partner']
    let results = [ui, customer]
    let choices = [uiChoices, customerChoices]

    const resumeButton = () => {
        window.open('https://docs.google.com/document/d/1NHRPvw4y2NBZ1Rd52Dm9ek9CZjjWjDPKq7od_7C7JN4/', '_blank');
    }

    const ticker = (index) => {
        let choice = 0
        results[index] = choices[index][choice]
        setInterval(() => {
            choice++
            if (choice > choices[index].length - 1){
                choice = 0;
            }
           results[index] = choices[index][choice]
   
        }, 200);
    }

    for (let i = 0; i < results.length; i++){
        ticker(i)
    }
</script>

<div class="container">
    <section>
        <div class="grp">
            <h1 class="welcome-hero">
              Howdy, friend.<span class="second"> <br> I'm Eric</span>.
            </h1>
            <p class="welcome-text">I'm a front-end developer who loves building <span aria-label="bold, inviting, accessible, inviting, whimsical, effective"></span><span class="descrip" aria-hidden="true" >{results[0]}</span> UI.
               I spent the first decade of my career building <span class="ayo1">customer</span> processes and have become an expert in the people on the other side of the screen. </p>
    
      <button class="primary" on:click={resumeButton}>View my resume.</button>
        </div>
    
        <div class="circle-3">
    
        </div>
        <div class="photo">
            <div class="circle"></div>
            <div class="circle"></div>
            <div class="circle"></div>
        </div>
    
    
    
    
    </section>
</div>



<style>
@import "open-props/style";
@import "open-props/normalize";
@import "open-props/masks/edges";

.container{
    background-image: var(--gradient-16);
}

.grp{
    width: 100%;
}


h1{
    color: var(--violet-7);
    line-height: var(--font-lineheight-1);
    font-size: var(--font-size-8);
    font-weight: var(--font-weight-9);
    font-family: var(--font-sans);
    margin-bottom: 0;
    /* text-shadow: 2px 3px 1px var(--blue-2); */
    /* background-image: var(--gradient-2);
    filter: var(--noise-filter-3);
    background-size: 1000px;

    -webkit-background-clip: text;
  -webkit-text-fill-color: transparent; */
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
    width: 40%;
    max-width: 500px;
    margin-right: var(--size-10);
    margin-top: var(--size-4);
    aspect-ratio: 1;
    animation: grad 20s linear 0s infinite alternate none;
    position: relative;
    background-position-x:0px;
    background-image: var(--gradient-2);
    filter: var(--noise-filter-2);
    background-size: 2000px 2000px;
    border-radius: 999px;
    z-index: 7;
    opacity: 1;
    display: grid;
    place-items: center;
}

.circle{
    width: 115%;
    aspect-ratio: 10;
    /* transform-origin: center; */
    transform: rotate(0deg);
    border-top: 3px dotted var(--yellow-4);
    border-left: 1px dashed var(--blue-4);
    border-right: 1px dashed var(--blue-6);
    border-radius: 50%;
    z-index: 200;
    mask-clip:  unset;
    animation: round 27s linear 0s infinite running none;
    opacity: 0.6;
    position: relative;
}

    .circle:nth-of-type(odd){
        width: 90%;
        /* position: absolute;
        top: 0;
        left: 0; */
        border-top: 2px dotted var(--pink-2);
        border-left: 2px dashed var(--pink-4);
        border-right: 2x dotted var(--pink-6);
        animation: roundy 30s linear 0s infinite running none;
        /* transform: translateX(-15%)translateY(150%) rotate(10deg); */
    }
    .circle:nth-of-type(1){
        /* position: absolute;
        top: 0;
        left: 0; */
        border-top: 7px dotted var(--pink-2);
        border-left: 7px dashed var(--pink-4);
        border-right: 7px dotted var(--pink-6);
        animation: roundy 7s linear 0s infinite running none;

        /* transform: translateX(-15%)translateY(320%) rotate(10deg); */

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

    .descrip{
  
        animation-duration: 5s;

        text-align: center;
        display: inline-block;
        width: 9ch;
        /* background-color: var(--gray-9); */
        color: var(--violet-7);
        font-weight: var(--font-weight-9);
    }
    .ayo1{
  
  animation-duration: 5s;

  text-align: center;
  display: inline-block;
  width: 8ch;
  /* background-color: var(--gray-9); */
  color: var(--violet-7);
  font-weight: var(--font-weight-9);
}

    section{
        max-width: 1500px;
        height: 100vh;
        margin: 0 auto;
        gap: var(--size-4);
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;

        padding: var(--size-7);
     
        line-height: var(--font-lineheight-0);
        /* -webkit-mask: var(--mask-edge-drip-bottom); */
   



    }

    button {
  /* background: white; */
  color: var(--violet-7);
  font-size: var(--font-size-3);
  padding-inline: var(--size-5);
  padding-block: var(--size-3);
  border-radius: var(--radius-2);
  box-shadow: var(--shadow-2);
  margin-top: var(--size-3);
  user-select: none;
}

a{
    user-select: none;
}

button.primary {
  background: var(--violet-7);
font-weight: var(--font-weight-7);
text-shadow: 0 1px 0 var(--red-2);
color: white;
border: 4px solid var(--violet-6);
}

button.primary:hover {
  background: var(--violet-5);
  color: var(--violet-0);
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
        transform:  rotate(-360deg);
    }
    76% {
    }
    100% {
        background-position: 00px -00px;
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
        transform:  rotate(360deg);
    }
    76% {
        border-top: 4px dotted var(--blue-4);
        border-left: 4px dotted var(--blue-6);
        border-right: 4px dotted var(--blue-8);
    }
    100% {

    }
}

@keyframes roundy{
    0% {
        border-top: 10px dotted var(--blue-3);
        border-left: 10px dotted var(--blue-6);
        border-right: 10px dotted var(--blue-8);
        transform: rotate(360 0 0);

    }
    22% {
        border-top: 2px dotted var(--indigo-5);
        border-left: 2px dotted var(--indigo-6);
        border-right: 2px dotted var(--indigo-8);
    }
    47% {
        transform: rotate(0 0 0);
        transform: perspective(500px) translate(10px, 0, 20px) rotateY(3deg);

    }
    50% {
        border-top: 5px dotted var(--indigo-5);
        border-left: 5px dotted var(--indigo-6);
        border-right: 5px dotted var(--indigo-8);
    }
    100% {

    }
}

@media (max-width: 800px){
    section{
        flex-direction: column-reverse;
    }

    .photo{
        margin:var(--size-3)0;
    }
}



@keyframes spin {
  from {
    transform: rotate(0);
  }
  to{
    transform: rotate(359deg);
  }
}

@keyframes spin3D {
  from {
    transform: rotate3d(.5,.5,.5, 360deg);
  }
  to{
    transform: rotate3d(0deg);
  }
}

@keyframes configure-clockwise {
  0% {
    transform: rotate(0);
  }
  25% {
    transform: rotate(90deg);
  }
  50% {
    transform: rotate(180deg);
  }
  75% {
    transform: rotate(270deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

@keyframes configure-xclockwise {
  0% {
    transform: rotate(45deg);
  }
  25% {
    transform: rotate(-45deg);
  }
  50% {
    transform: rotate(-135deg);
  }
  75% {
    transform: rotate(-225deg);
  }
  100% {
    transform: rotate(-315deg);
  }
}

@keyframes pulse {
  from {
    opacity: 1;
    transform: scale(1);
  }
  to {
    opacity: .25;
    transform: scale(.75);
  }
}


</style>