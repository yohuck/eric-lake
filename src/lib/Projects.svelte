<script>
import Popper from "./popper.svelte";
import Card from "./Card.svelte"
</script>

<section>
   
    <article>
        <div class="info">
            <h4>Habit Stack</h4>
            <hr>
            <div class="grp">
                <a href="github.com">GitHub Repo</a>
                <a href="github.com">Live Site</a>
            </div>
            <p>A full stack application that helps build habit that stick through repetition and reward.</p>
            <ul>
                <li>MySql</li>
                <li>Express</li>
                <li>Handlebars</li>
                <li>Sequelize</li>
                <li>Node.js</li>
                <li>Authentication</li>
            </ul>
        </div>
    </article>
    <article>
        <div class="info">
            <h4>Recycle Better</h4>
            <hr>
            <div class="grp">
                <a target='blank' href="https://github.com/yohuck/wish-cycle">GitHub Repo</a>
                <a target="blank" href="https://yohuck.github.io/wish-cycle/">Live Site</a>
            </div>
            <p>A web application to help conscious consumers quickly and easily find the best way to recycle or dispose of household items.</p>
            <ul>
                <li>JQuery</li>
                <li>Socrate Open API</li>
                <li>Geolocation API</li>
                <li>Bulma</li>
                <li>JavaScript</li>
            </ul>
        </div>
    </article>
    <article>
        <div class="info">
            <h4>City Weather</h4>
            <hr>
            <div class="grp">
                <a target='blank' href="https://github.com/yohuck/city-weather">GitHub Repo</a>
                <a target="blank" href="https://yohuck.github.io/city-weather/">Live Site</a>
            </div>
            <p>A web application using the OpenWeather API to find and store weather information.</p>
            <ul>
                <li>OpenWeather API</li>
                <li>JavaScript</li>
                <li>CSS3</li>
                <li>HTML5</li>
            </ul>
        </div>
    </article>
    <article class="pop">
        <div class="info">
            <h4>Popper Toy</h4>
            <hr>
            <div class="grp">
                <a target='blank' href="https://github.com/yohuck/wish-cycle">Codepen</a>
            </div>
        </div>
        <Popper />
    </article>
  
    <article class="card">
        <div class="info">
            <h4>Chip Card Button</h4>
            <hr>
            <div class="grp">
                <a target='blank' href="https://github.com/yohuck/wish-cycle">CodePen</a>
            </div>
        </div>
        <Card />
    </article>



</section>

<style>

    .pop{
        display: flex;
        justify-content: center;
        flex-direction: column;
        justify-content: space-between;
    }

    .card{
        display: flex;
        flex-direction: column;
        justify-content: space-between;

    }

    section{
        background-image: var(--gradient-2);
    background-size: 3000px 3000px;


        padding: var(--size-3);
        width: 100%;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 2fr));
        grid-gap: var(--size-2);
    }

    hr{
       background-color: var(--violet-7);
       height: 3px;
       border-radius: var(--border-size-3);
    }

    code{
        max-width: 100%;
        
        word-wrap: normal;
        flex-wrap: wrap;
    }

    p{

        color: var(--gray-1);
        padding: var(--size-1);
        border-radius: var(--border-size-3);
    }

    hr{
        margin: 1rem 0;
    }

    article{
        /* background-image: var(--gradient-8); */
        background-color: black;
        
        border: 1px solid black;
        border-radius: var(--radius-conditional-3);
        padding: var(--size-3);
        box-shadow: var(--shadow-3);
        border: var(--border-size-3) solid transparent                      ;
        color: var(--violet-2)
        /* max-width: 2fr; */
    }

    h1{ 
        margin: 0;
        padding: 0;
        width: 100%;
        text-align: center;
        -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
    }

    h4{
        color: var(--violet-2);
    }

    a{
        margin: 0;
        padding: 0;
    }

    .grp{
        padding: 2px solid red;
        margin: 0;
    }



    article:hover, article:focus{
        border: var(--border-size-3) solid var(--red-6 );              
        box-shadow: var(--shadow-4);
    }

    .photo{
        display: flex;
    }

    img{
        width: 100%;

    }
</style>