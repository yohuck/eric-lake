<script>
import Popper from "./popper.svelte";
import Card from "./Card.svelte"

</script>
<!-- <section class="backdrop title">
    <h2>Check out my work:<br><span></span></h2>
</section> -->
<div class="con">
    <section class="backdrop">
    
        <article >
            <div class="info">
                <div class="top">
                    <h4>Habit Stack</h4>
                    <hr>
                    <div class="grp">
                        <a href="https://github.com/yohuck/habit-map" target="_blank">GitHub Repo</a>
                        <a href="https://habitstack.herokuapp.com/" target="_blank">Live Site</a>
                    </div>
                    <p>A full stack application that helps build habit that stick through repetition and reward.</p>
                </div>
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
                <div class="top">
                    <h4>Recycle Better</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://github.com/yohuck/wish-cycle">GitHub Repo</a>
                        <a target="blank" href="https://yohuck.github.io/wish-cycle/">Live Site</a>
                    </div>
                    <p>A web application to help conscious consumers quickly and easily find the best way to recycle or dispose of household items.</p>
                </div>
                <div class="btm">
    
                    <ul>
                        <li>JQuery</li>
                        <li>Socrata Open API</li>
                        <li>Geolocation API</li>
                        <li>Bulma</li>
                        <li>JavaScript</li>
                    </ul>
                    <!-- <img src="../src/assets/a.gif" alt=""> -->
                            </div>
                </div>
        </article>
        <article>
            <div class="info">
                <div class="top">
                    <h4>City Weather</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://github.com/yohuck/city-weather">GitHub Repo</a>
                        <a target="blank" href="https://yohuck.github.io/city-weather/">Live Site</a>
                    </div>
                    <p>A web application using the OpenWeather API to find and store weather information.</p>
                </div>
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
                    <a target='blank' href="https://codepen.io/yohuck/pen/bGaLKaW">Codepen</a>
                </div>
            </div>
            <Popper />
        </article>
    
        <article class="card">
            <div class="top">
                <div class="info">
                    <h4>Chip Card Button</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://codepen.io/yohuck/pen/dyJZXxQ">CodePen</a>
                    </div>
                </div>
            </div>
            <Card />
        </article>
    
    
    
    </section>
</div>

<style>
    @import "open-props/colors-hsl";
*{
    box-sizing: border-box;
}

.con{
    background-color: hsl(var(--indigo-9-hsl) / 100%);
}
    .pop{
        display: flex;
        justify-content: center;
        flex-direction: column;
        justify-content: space-between;
    }

    .btm{
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
    }


    .card{
        display: flex;
        flex-direction: column;
        justify-content: space-between;

    }



.backdrop {
  background-color: hsl(var(--indigo-9-hsl) / 90%);
}

    section{
        background-color: hsl(var(--gray-3-hsl) / 30%);
        background-size: 3000px 3000px;
        max-width:92%;
        margin: 0 auto;

        
        padding: var(--size-3);

        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: var(--size-2);
    }

    hr{
       background-color: var(--indigo-4);
       height: 3px;
       border-radius: var(--border-size-3);
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
        /* height: 100%; */
        /* border: 1px solid black; */
        border-radius: var(--radius-conditional-3);
        padding: var(--size-3);
        box-shadow: var(--shadow-3);
        margin: 0;
        border: var(--border-size-3) solid transparent;
        color: var(--violet-2);
       
        /* max-width: 2fr; */
    }

    h2{ 
        margin: 0;
        padding: 0;
        /* width: 100%; */
        color: var(--indigo-2);
        background-color: black;
        border-radius: var(--radius-conditional-3);
        padding: var(--size-2);
        box-shadow: var(--shadow-3);
        border: var(--border-size-3) solid transparent;

        /* -webkit-background-clip: text;
  -webkit-text-fill-color: transparent; */
    }

    span{
        font-size: var(--font-size-2);
    }

    h4{
        color: var(--indigo-2);
    }

    a{
        margin: 0;
        padding: 0;
    }


    ul{
        width: 100%;
        flex-wrap: wrap;
        margin: 0;
        padding: 0;
        display: flex;
        gap: var(--size-1);
    }

    ul li{
        color: white;
        list-style: none;
        padding: var(--size-1);
        background-color: var(--indigo-6);
        border-radius: var(--border-size-3);
    }



    article:hover, article:focus{
        border: var(--border-size-3) solid var(--red-6 );              
        box-shadow: var(--shadow-4);
    }



    .info{
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
</style>