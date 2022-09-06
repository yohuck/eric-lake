<header>
    <nav>
        <div class="photo">
            <div class="circle"></div>
            <div class="circle"></div>
            <div class="circle"></div>
        </div>
    
        <ul>
            <li>About</li>
            <li>Work</li>
            <li>Stack</li>
            <li>Contact</li>
        </ul>
    </nav>
</header>

<style>

.photo{
    margin: var(--size-2) var(--size-5);
    width: 50px;
    aspect-ratio: 1;
    animation: grady 20s linear 0s infinite alternate none;
    position: relative;
    background-position-x:0px;
    background-image: var(--gradient-2);
    filter: var(--noise-filter-2);
    background-size: 300px 300px;
    border-radius: 999px;
    z-index: 7;
    opacity: 0.2;
    display: grid;
    place-items: center;
}

.photo:hover, .photo:focus{
    opacity: 0.7
}

.circle{
    width: 115%;
    aspect-ratio: 10;
    /* transform-origin: center; */
    transform: rotate(0deg);
    border-top: 1px dotted var(--yellow-4);
    border-left: 1px dashed var(--blue-4);
    border-right: 1px dashed var(--blue-6);
    border-radius: 50%;
    z-index: 100;
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
        border-top: 1px dotted var(--pink-2);
        border-left: 1px dashed var(--pink-4);
        border-right: 1px dotted var(--pink-6);
        animation: roundy 30s linear 0s infinite running none;
        /* transform: translateX(-15%)translateY(150%) rotate(10deg); */
    }
    .circle:nth-of-type(1){
        /* position: absolute;
        top: 0;
        left: 0; */
        border-top: 1px dotted var(--pink-2);
        border-left: 1px dashed var(--pink-4);
        border-right: 1px dotted var(--pink-6);
        animation: roundy 7s linear 0s infinite running none;

        /* transform: translateX(-15%)translateY(320%) rotate(10deg); */

    }

nav{
    background-color: rgba(11, 11, 11, 0.076);
    width: 100%;
    position: fixed;
    z-index: 10000;
    animation: grad 10s linear 0s infinite alternate none;
    display: flex;
    justify-content: space-between;
}

nav ul{
    text-align: center;
    padding: var(--size-1);
    margin: var(--size-1);
    /* max-width: 1500px; */
    display: flex;
    gap: 1rem;
    justify-content: flex-end;
}

li{
    margin: 0;
    padding: var(--size-1);
    font-weight: var(--font-weight-8);
    /* margin: var(--size-2); */
    list-style: none;
    color: var(--grape-2);
    border-bottom: 4px dotted transparent;
    background-image: var(--gradient-2);
    filter: var(--noise-filter-3);
    /* background-size: 1000px; */

    -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

li:hover, li:active{
    border-bottom: 4px dotted var(--grape-5);
}


@keyframes grad{
    0% {
        background-position: -1000px -2000px;
    }
    22% {
    }
    47% {

    }
    76% {
    }
    100% {
        background-position: 0px 0px;
    }
}
@keyframes grady{
    0% {
        background-position: -100px -100px;
    }
    22% {
    }
    47% {
        transform: rotate(360deg);
    }
    76% {
    }
    100% {
        background-position: 0px 0px;
    }
}
</style>