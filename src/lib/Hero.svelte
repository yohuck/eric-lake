<script>
    let ui = '';
    let uiChoices = ['b','bo','bol','bold', 'bold','bold', 'bold', 'i', 'in', 'inv', 'invi', 'invit', 'inviti', 'invitin', 'inviting', 'inviting', 'inviting', 'inviting', 'a', 'ac','acc','acce','acces','access','accessi','accessib','accessibl','accessible', 'accessible','accessible', 'accessible','w','wh','whi','whim','whims','whimsi','whimsic','whimsica','whimsical', 'whimsical','whimsical', 'whimsical','e','ef','eff','effe','effec','effect','effecti','effectiv','effective', 'effective','effective', 'effective']
    let customer = '';
    let customerChoices = ['c','cu','cus','cust','custo','custom','custome','customer','customer','customer','customer','customer','customer', 'u', 'us','use','user','user','user','user','user','c','cl','cli','clie','clien','client','client','client','client','client', 'p', 'pa', 'par', 'part', 'partn', 'partne', 'partner', 'partner', 'partner', 'partner', 'partner', 'partner']
    let results = [ui, customer]
    let choices = [uiChoices, customerChoices]

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

<section>
    <div class="grp">
        <h1 class="welcome-hero">
          Howdy, friend.<span class="second"> <br> I'm Eric</span>.
        </h1>
        <p class="welcome-text">I'm a front-end developer who loves building <span class="ayo">{results[0]}</span> UI. 
           I spent the first decade of my career building <span class="ayo1">customer</span> processes and have become an expert in the people on the other side of the screen. </p>
        
           <a target="_blank" href="https://docs.google.com/document/d/1NHRPvw4y2NBZ1Rd52Dm9ek9CZjjWjDPKq7od_7C7JN4/edit?usp=sharing"><button class="primary">View my resume.</button></a>
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
 
         color: var(--grape-8);
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
  
        animation-duration: 5s;

        text-align: center;
        display: inline-block;
        width: 9ch;
        /* background-color: var(--gray-9); */
        color: var(--grape-8);
        font-weight: var(--font-weight-9);
    }
    .ayo1{
  
  animation-duration: 5s;

  text-align: center;
  display: inline-block;
  width: 8ch;
  /* background-color: var(--gray-9); */
  color: var(--grape-8);
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
  background: var(--indigo-8);
  font-weight: var(--font-weight-7);
  text-shadow: 0 1px 0 var(--red-2);
  color: white;
}

button.primary:hover {
  background: var(--grape-8);
  color: var(--indigo-1);
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