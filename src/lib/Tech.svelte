<!-- <div class="container">
    <section>
        <h2>Tech Stack</h2>

        <ul class="solar-system">
            <li class="sun">
                <h3 >
                    Front End
                </h3>
                <ul class="orbit">
                    <li class="green-orbit white-orbit">Svelte</li>
                    <li class="venus-orbit orbit">React</li>
                    <li>Handlebars</li>
                </ul>
                <ul>
                    <li>Boopstrap</li>
                    <li>Bulma</li>
                    <li>Open-Props</li>
                </ul>
            </li>
        </ul>
    </section>
</div> -->

<style>
ul{
    list-style: none;
    display: flex;
}


ul ul{
    width: 100%;
    display: grid;
    grid-auto-flow: column;
}

ul ul li{
width: 2rem;
height: 2rem;
padding: var(--size-2);
margin: var(--size-2);
border-radius: var(--border-radius-3);
background-image: var(--gradient-7);
/* filter: var(--noise-filter-1); */
background-size: cover;
box-shadow: var(--shadow-6);
color: var(--orange-0);
font-weight: var(--font-weight-6);
display: grid;
font-family: var(--font-mono);
font-size: var(--size-3);
place-items: center;
border-radius: var(--radius-blob-5);
}

ul li li:nth-child(1){
    border-radius: var(--radius-blob-1);
}
ul li li:nth-child(2){
    border-radius: var(--radius-blob-2);
}
ul li li:nth-child(3){
    border-radius: var(--radius-blob-3);
}

</style>